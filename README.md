flowchart LR;
    main-->|Logged In| bottom
    main-->|Not Logged In| login
    login-->otp
    otp-->switch
    switch-->bottom
    bottom-->home
    bottom-->services
    bottom-->family
    bottom-->settings
    bottom-->icon
    icon-->vision
    home-->navbar
    navbar-->language
    navbar-->notification
    navbar-->profile
    home-->cards
    cards-->barcode
    home-->status
    home-->actions
    actions-->prescription
    actions-->treatment
    actions-->awareness
    actions-->tips
    actions-->facts
    services-->servicelist
    servicelist-->prescription
    servicelist-->connect
    servicelist-->otherservices
    settings-->viewprofile
    settings-->notification
    settings-->terms
    settings-->privacy
    settings-->about
    settings-->logout
