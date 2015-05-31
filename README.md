# tinker

Access Statamic from the CLI

Install with

    cd <statamic site root>
    git clone https://github.com/gazsp/tinker.git
    cd tinker
    composer install


The run with (from your site root)

    tinker/tinker.php

You can now access Statamic from the command line. E.g:

    Statamic> $members = MemberService::getMembers()->get();
    // ...
    Statamic> reset($members);
    // array(
    //   'first_name' => 'Gary',
    //   'last_name' => 'Pearman',
    //   'roles' => array(
    //     0 => 'member',
    //     1 => 'admin'
    //   ),
    // ...
    //   'first' => true,
    //   'last' => false,
    //   'count' => 1,
    //   'total_results' => 116,
    //   'biography_raw' => '',
    //   'biography' => ''
    // )
    Statamic>
