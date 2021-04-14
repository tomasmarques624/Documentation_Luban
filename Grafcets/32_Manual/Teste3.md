$menu = Menu::handler('mailbox'); 

// items
$menu
    ->add('contacts', 'Contacts')
    ->add('inbox', 'Inbox')
    ->raw(null, null, ['class' => 'divider'])
    ->add('folders', 'Folders', Menu::items() 
        ->prefixParents() 
        ->add('urgent', 'Urgent') // with prefix: /folders/urgent
        ->add('sent', 'Sent')
        ->add('deleted', 'Deleted')
    );

// styling
$menu
    ->addClass('nav navbar-nav')
    ->getItemsByContentType(Menu\Items\Contents\Link::class)
    ->map(function($item) {
        if ( $item->isActive() )  {
            $item->addClass('active');
        }
    });
