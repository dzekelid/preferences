---
swagger: "2.0"
x-collection-name: Trello
x-complete: 0
info:
  title: Trello Put Boards Preferences Comments
  description: Put boards preferences comments.
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