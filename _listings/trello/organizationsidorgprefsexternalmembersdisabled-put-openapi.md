---
swagger: "2.0"
x-collection-name: Trello
x-complete: 0
info:
  title: Trello Put Organizations Preferences Externalmembersdisabled
  description: Put organizations preferences externalmembersdisabled.
  termsOfService: https://trello.com/legal
  contact:
    name: Trello
    url: https://trello.com/home
  version: "1.0"
host: trello.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /boards/{idBoard}/myPrefs:
    get:
      summary: Get Boards My Preferences
      description: Get boards my preferences.
      operationId: getBoardsMyPrefsByIdBoard
      x-api-path-slug: boardsidboardmyprefs-get
      parameters:
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - My
      - Preferences
  /boards/{idBoard}/myPrefs/emailPosition:
    put:
      summary: Put Boards My Preferences Emailposition
      description: Put boards my preferences emailposition.
      operationId: updateBoardsMyPrefsEmailPositionByIdBoard
      x-api-path-slug: boardsidboardmyprefsemailposition-put
      parameters:
      - in: body
        name: body
        description: Attributes of My Prefs Email Position to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - My
      - Preferences
      - Emailposition
  /boards/{idBoard}/myPrefs/idEmailList:
    put:
      summary: Put Boards My Preferences Emaillist
      description: Put boards my preferences emaillist.
      operationId: updateBoardsMyPrefsIdEmailListByIdBoard
      x-api-path-slug: boardsidboardmyprefsidemaillist-put
      parameters:
      - in: body
        name: body
        description: Attributes of My Prefs Id Email List to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - My
      - Preferences
      - Emaillist
  /boards/{idBoard}/myPrefs/showListGuide:
    put:
      summary: Put Boards My Preferences Showlistgue
      description: Put boards my preferences showlistgue.
      operationId: updateBoardsMyPrefsShowListGuideByIdBoard
      x-api-path-slug: boardsidboardmyprefsshowlistguide-put
      parameters:
      - in: body
        name: body
        description: Attributes of My Prefs Show List Guide to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - My
      - Preferences
      - Showlistgue
  /boards/{idBoard}/myPrefs/showSidebar:
    put:
      summary: Put Boards My Preferences Show Sidebar
      description: Put boards my preferences show sidebar.
      operationId: updateBoardsMyPrefsShowSidebarByIdBoard
      x-api-path-slug: boardsidboardmyprefsshowsidebar-put
      parameters:
      - in: body
        name: body
        description: Attributes of My Prefs Show Sidebar to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - My
      - Preferences
      - Show
      - Sidebar
  /boards/{idBoard}/myPrefs/showSidebarActivity:
    put:
      summary: Put Boards My Preferences Show Sidebar Activity
      description: Put boards my preferences show sidebar activity.
      operationId: updateBoardsMyPrefsShowSidebarActivityByIdBoard
      x-api-path-slug: boardsidboardmyprefsshowsidebaractivity-put
      parameters:
      - in: body
        name: body
        description: Attributes of My Prefs Show Sidebar Activity to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - My
      - Preferences
      - Show
      - Sidebar
      - Activity
  /boards/{idBoard}/myPrefs/showSidebarBoardActions:
    put:
      summary: Put Boards My Preferences Show Sidebar Board Actions
      description: Put boards my preferences show sidebar board actions.
      operationId: updateBoardsMyPrefsShowSidebarBoardActionsByIdBoard
      x-api-path-slug: boardsidboardmyprefsshowsidebarboardactions-put
      parameters:
      - in: body
        name: body
        description: Attributes of My Prefs Show Sidebar Board Actions to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - My
      - Preferences
      - Show
      - Sidebar
      - Board
      - Actions
  /boards/{idBoard}/myPrefs/showSidebarMembers:
    put:
      summary: Put Boards My Preferences Show Sidebarmembers
      description: Put boards my preferences show sidebarmembers.
      operationId: updateBoardsMyPrefsShowSidebarMembersByIdBoard
      x-api-path-slug: boardsidboardmyprefsshowsidebarmembers-put
      parameters:
      - in: body
        name: body
        description: Attributes of My Prefs Show Sidebar Members to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - My
      - Preferences
      - Show
      - Sidebarmembers
  /boards/{idBoard}/prefs/background:
    put:
      summary: Put Boards Preferences Background
      description: Put boards preferences background.
      operationId: updateBoardsPrefsBackgroundByIdBoard
      x-api-path-slug: boardsidboardprefsbackground-put
      parameters:
      - in: body
        name: body
        description: Attributes of Prefs Background to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Preferences
      - Background
  /boards/{idBoard}/prefs/calendarFeedEnabled:
    put:
      summary: Put Boards Preferences Calendar Feed Enabled
      description: Put boards preferences calendar feed enabled.
      operationId: updateBoardsPrefsCalendarFeedEnabledByIdBoard
      x-api-path-slug: boardsidboardprefscalendarfeedenabled-put
      parameters:
      - in: body
        name: body
        description: Attributes of Prefs Calendar Feed Enabled to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Preferences
      - Calendar
      - Feed
      - Enabled
  /boards/{idBoard}/prefs/cardAging:
    put:
      summary: Put Boards Preferences Cardaging
      description: Put boards preferences cardaging.
      operationId: updateBoardsPrefsCardAgingByIdBoard
      x-api-path-slug: boardsidboardprefscardaging-put
      parameters:
      - in: body
        name: body
        description: Attributes of Prefs Card Aging to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Preferences
      - Cardaging
  /boards/{idBoard}/prefs/cardCovers:
    put:
      summary: Put Boards Preferences Cardcovers
      description: Put boards preferences cardcovers.
      operationId: updateBoardsPrefsCardCoversByIdBoard
      x-api-path-slug: boardsidboardprefscardcovers-put
      parameters:
      - in: body
        name: body
        description: Attributes of Prefs Card Covers to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Preferences
      - Cardcovers
  /boards/{idBoard}/prefs/comments:
    put:
      summary: Put Boards Preferences Comments
      description: Put boards preferences comments.
      operationId: updateBoardsPrefsCommentsByIdBoard
      x-api-path-slug: boardsidboardprefscomments-put
      parameters:
      - in: body
        name: body
        description: Attributes of Prefs Comments to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Preferences
      - Comments
  /boards/{idBoard}/prefs/invitations:
    put:
      summary: Put Boards Preferences Invitations
      description: Put boards preferences invitations.
      operationId: updateBoardsPrefsInvitationsByIdBoard
      x-api-path-slug: boardsidboardprefsinvitations-put
      parameters:
      - in: body
        name: body
        description: Attributes of Prefs Invitations to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Preferences
      - Invitations
  /boards/{idBoard}/prefs/permissionLevel:
    put:
      summary: Put Boards Preferences Permissionlevel
      description: Put boards preferences permissionlevel.
      operationId: updateBoardsPrefsPermissionLevelByIdBoard
      x-api-path-slug: boardsidboardprefspermissionlevel-put
      parameters:
      - in: body
        name: body
        description: Attributes of Prefs Permission Level to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Preferences
      - Permissionlevel
  /boards/{idBoard}/prefs/selfJoin:
    put:
      summary: Put Boards Preferences Selfjoin
      description: Put boards preferences selfjoin.
      operationId: updateBoardsPrefsSelfJoinByIdBoard
      x-api-path-slug: boardsidboardprefsselfjoin-put
      parameters:
      - in: body
        name: body
        description: Attributes of Prefs Self Join to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Preferences
      - Selfjoin
  /boards/{idBoard}/prefs/voting:
    put:
      summary: Put Boards Preferences Voting
      description: Put boards preferences voting.
      operationId: updateBoardsPrefsVotingByIdBoard
      x-api-path-slug: boardsidboardprefsvoting-put
      parameters:
      - in: body
        name: body
        description: Attributes of Prefs Voting to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Preferences
      - Voting
  /members/{idMember}/prefs/colorBlind:
    put:
      summary: Put Members Preferences Colorblind
      description: Put members preferences colorblind.
      operationId: updateMembersPrefsColorBlindByIdMember
      x-api-path-slug: membersidmemberprefscolorblind-put
      parameters:
      - in: body
        name: body
        description: Attributes of Prefs Color Blind to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Preferences
      - Colorblind
  /members/{idMember}/prefs/locale:
    put:
      summary: Put Members Preferences Locale
      description: Put members preferences locale.
      operationId: updateMembersPrefsLocaleByIdMember
      x-api-path-slug: membersidmemberprefslocale-put
      parameters:
      - in: body
        name: body
        description: Attributes of Prefs Locale to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Preferences
      - Locale
  /members/{idMember}/prefs/minutesBetweenSummaries:
    put:
      summary: Put Members Preferences Minutesbetweensummaries
      description: Put members preferences minutesbetweensummaries.
      operationId: updateMembersPrefsMinutesBetweenSummariesByIdMember
      x-api-path-slug: membersidmemberprefsminutesbetweensummaries-put
      parameters:
      - in: body
        name: body
        description: Attributes of Prefs Minutes Between Summaries to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Preferences
      - Minutesbetweensummaries
  /organizations/{idOrg}/prefs/associatedDomain:
    delete:
      summary: Delete Organizations Preferences Associateddomain
      description: Delete organizations preferences associateddomain.
      operationId: deleteOrganizationsPrefsAssociatedDomainByIdOrg
      x-api-path-slug: organizationsidorgprefsassociateddomain-delete
      parameters:
      - in: path
        name: idOrg
        description: idOrg or name
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Preferences
      - Associateddomain
    put:
      summary: Put Organizations Preferences Associateddomain
      description: Put organizations preferences associateddomain.
      operationId: updateOrganizationsPrefsAssociatedDomainByIdOrg
      x-api-path-slug: organizationsidorgprefsassociateddomain-put
      parameters:
      - in: body
        name: body
        description: Attributes of Prefs Associated Domain to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idOrg
        description: idOrg or name
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Preferences
      - Associateddomain
  /organizations/{idOrg}/prefs/boardVisibilityRestrict/org:
    put:
      summary: Put Organizations Preferences Boardvisibilityrestrict Org
      description: Put organizations preferences boardvisibilityrestrict org.
      operationId: updateOrganizationsPrefsBoardVisibilityRestrictOrgByIdOrg
      x-api-path-slug: organizationsidorgprefsboardvisibilityrestrictorg-put
      parameters:
      - in: body
        name: body
        description: Attributes of Prefs Board Visibility Restrict to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idOrg
        description: idOrg or name
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Preferences
      - Boardvisibilityrestrict
      - Org
  /organizations/{idOrg}/prefs/boardVisibilityRestrict/private:
    put:
      summary: Put Organizations Preferences Boardvisibilityrestrict Private
      description: Put organizations preferences boardvisibilityrestrict private.
      operationId: updateOrganizationsPrefsBoardVisibilityRestrictPrivateByIdOrg
      x-api-path-slug: organizationsidorgprefsboardvisibilityrestrictprivate-put
      parameters:
      - in: body
        name: body
        description: Attributes of Prefs Board Visibility Restrict to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idOrg
        description: idOrg or name
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Preferences
      - Boardvisibilityrestrict
      - Private
  /organizations/{idOrg}/prefs/boardVisibilityRestrict/public:
    put:
      summary: Put Organizations Preferences Boardvisibilityrestrict Public
      description: Put organizations preferences boardvisibilityrestrict public.
      operationId: updateOrganizationsPrefsBoardVisibilityRestrictPublicByIdOrg
      x-api-path-slug: organizationsidorgprefsboardvisibilityrestrictpublic-put
      parameters:
      - in: body
        name: body
        description: Attributes of Prefs Board Visibility Restrict to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idOrg
        description: idOrg or name
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Preferences
      - Boardvisibilityrestrict
      - Public
  /organizations/{idOrg}/prefs/externalMembersDisabled:
    put:
      summary: Put Organizations Preferences Externalmembersdisabled
      description: Put organizations preferences externalmembersdisabled.
      operationId: updateOrganizationsPrefsExternalMembersDisabledByIdOrg
      x-api-path-slug: organizationsidorgprefsexternalmembersdisabled-put
      parameters:
      - in: body
        name: body
        description: Attributes of Prefs External Members Disabled to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idOrg
        description: idOrg or name
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Preferences
      - Externalmembersdisabled
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---