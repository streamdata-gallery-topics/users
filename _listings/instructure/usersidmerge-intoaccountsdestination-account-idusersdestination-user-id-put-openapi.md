---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Users API Merge user into another user
  description: Merge user into another user.
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/activity_stream:
    get:
      summary: List the activity stream
      description: List the activity stream.
      operationId: list-the-activity-stream
      x-api-path-slug: usersactivity-stream-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Activity
      - Stream
  /users/self/activity_stream:
    delete:
      summary: Hide all stream items
      description: Hide all stream items.
      operationId: hide-all-stream-items
      x-api-path-slug: usersselfactivity-stream-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Activity
      - Stream
    get:
      summary: List the activity stream
      description: List the activity stream.
      operationId: list-the-activity-stream
      x-api-path-slug: usersselfactivity-stream-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Activity
      - Stream
  /users/self/activity_stream/summary:
    get:
      summary: Activity stream summary
      description: Activity stream summary.
      operationId: activity-stream-summary
      x-api-path-slug: usersselfactivity-streamsummary-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Activity
      - Stream
      - Summary
  /users/self/activity_stream/{id}:
    delete:
      summary: Hide a stream item
      description: Hide a stream item.
      operationId: hide-a-stream-item
      x-api-path-slug: usersselfactivity-streamid-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Activity
      - Stream
      - Id
  /users/self/bookmarks:
    get:
      summary: List bookmarks
      description: List bookmarks.
      operationId: list-bookmarks
      x-api-path-slug: usersselfbookmarks-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Bookmarks
    post:
      summary: Create bookmark
      description: Create bookmark.
      operationId: create-bookmark
      x-api-path-slug: usersselfbookmarks-post
      parameters:
      - in: query
        name: data
        description: The data associated with the bookmark
      - in: query
        name: name
        description: The name of the bookmark
      - in: query
        name: position
        description: The position of the bookmark
      - in: query
        name: url
        description: The url of the bookmark
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Bookmarks
  /users/self/bookmarks/{id}:
    delete:
      summary: Delete bookmark
      description: Delete bookmark.
      operationId: delete-bookmark
      x-api-path-slug: usersselfbookmarksid-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Bookmarks
      - Id
    get:
      summary: Get bookmark
      description: Get bookmark.
      operationId: get-bookmark
      x-api-path-slug: usersselfbookmarksid-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Bookmarks
      - Id
    put:
      summary: Update bookmark
      description: Update bookmark.
      operationId: update-bookmark
      x-api-path-slug: usersselfbookmarksid-put
      parameters:
      - in: query
        name: data
        description: The data associated with the bookmark
      - in: query
        name: name
        description: The name of the bookmark
      - in: query
        name: position
        description: The position of the bookmark
      - in: query
        name: url
        description: The url of the bookmark
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Bookmarks
      - Id
  /users/self/communication_channels/{communication_channel_id}/notification_preferences:
    put:
      summary: Update multiple preferences
      description: Update multiple preferences.
      operationId: update-multiple-preferences
      x-api-path-slug: usersselfcommunication-channelscommunication-channel-idnotification-preferences-put
      parameters:
      - in: query
        name: notification_preferences[X][frequency]
        description: The desired frequency for &lt;X&gt; notification
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Communication
      - Channels
      - Communication
      - Channel
      - Id
      - Notification
      - Preferences
  /users/self/communication_channels/{communication_channel_id}/notification_preferences/notification:
    put:
      summary: Update a preference
      description: Update a preference.
      operationId: update-a-preference
      x-api-path-slug: usersselfcommunication-channelscommunication-channel-idnotification-preferencesnotification-put
      parameters:
      - in: query
        name: notification_preferences[frequency]
        description: The desired frequency for this notification
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Communication
      - Channels
      - Communication
      - Channel
      - Id
      - Notification
      - Preferences
      - Notification
  /users/self/communication_channels/{communication_channel_id}/notification_preference_categories/category:
    put:
      summary: Update preferences by category
      description: Update preferences by category.
      operationId: update-preferences-by-category
      x-api-path-slug: usersselfcommunication-channelscommunication-channel-idnotification-preference-categoriescategory-put
      parameters:
      - in: query
        name: category
        description: The name of the category
      - in: query
        name: notification_preferences[frequency]
        description: The desired frequency for each notification in the category
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Communication
      - Channels
      - Communication
      - Channel
      - Id
      - Notification
      - Preference
      - Categories
      - Category
  /users/self/communication_channels/{type}/address/notification_preferences:
    put:
      summary: Update multiple preferences
      description: Update multiple preferences.
      operationId: update-multiple-preferences
      x-api-path-slug: usersselfcommunication-channelstypeaddressnotification-preferences-put
      parameters:
      - in: query
        name: notification_preferences[X][frequency]
        description: The desired frequency for &lt;X&gt; notification
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Communication
      - Channels
      - Type
      - Address
      - Notification
      - Preferences
  /users/self/communication_channels/{type}/address/notification_preferences/{notification}:
    put:
      summary: Update a preference
      description: Update a preference.
      operationId: update-a-preference
      x-api-path-slug: usersselfcommunication-channelstypeaddressnotification-preferencesnotification-put
      parameters:
      - in: query
        name: notification_preferences[frequency]
        description: The desired frequency for this notification
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Communication
      - Channels
      - Type
      - Address
      - Notification
      - Preferences
      - Notification
  /users/self/course_nicknames:
    delete:
      summary: Clear course nicknames
      description: Clear course nicknames.
      operationId: clear-course-nicknames
      x-api-path-slug: usersselfcourse-nicknames-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Course
      - Nicknames
    get:
      summary: List course nicknames
      description: List course nicknames.
      operationId: list-course-nicknames
      x-api-path-slug: usersselfcourse-nicknames-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Course
      - Nicknames
  /users/self/course_nicknames/{course_id}:
    delete:
      summary: Remove course nickname
      description: Remove course nickname.
      operationId: remove-course-nickname
      x-api-path-slug: usersselfcourse-nicknamescourse-id-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Course
      - Nicknames
      - Course
      - Id
    get:
      summary: Get course nickname
      description: Get course nickname.
      operationId: get-course-nickname
      x-api-path-slug: usersselfcourse-nicknamescourse-id-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Course
      - Nicknames
      - Course
      - Id
    put:
      summary: Set course nickname
      description: Set course nickname.
      operationId: set-course-nickname
      x-api-path-slug: usersselfcourse-nicknamescourse-id-put
      parameters:
      - in: query
        name: nickname
        description: The nickname to set
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Course
      - Nicknames
      - Course
      - Id
  /users/self/favorites/courses:
    delete:
      summary: Reset course favorites
      description: Reset course favorites.
      operationId: reset-course-favorites
      x-api-path-slug: usersselffavoritescourses-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Courses
    get:
      summary: List favorite courses
      description: List favorite courses.
      operationId: list-favorite-courses
      x-api-path-slug: usersselffavoritescourses-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Courses
  /users/self/favorites/courses/{id}:
    delete:
      summary: Remove course from favorites
      description: Remove course from favorites.
      operationId: remove-course-from-favorites
      x-api-path-slug: usersselffavoritescoursesid-delete
      parameters:
      - in: query
        name: id
        description: the ID or SIS ID of the course to remove
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Courses
      - Id
    post:
      summary: Add course to favorites
      description: Add course to favorites.
      operationId: add-course-to-favorites
      x-api-path-slug: usersselffavoritescoursesid-post
      parameters:
      - in: query
        name: id
        description: The ID or SIS ID of the course to add
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Courses
      - Id
  /users/self/favorites/groups:
    delete:
      summary: Reset group favorites
      description: Reset group favorites.
      operationId: reset-group-favorites
      x-api-path-slug: usersselffavoritesgroups-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Groups
    get:
      summary: List favorite groups
      description: List favorite groups.
      operationId: list-favorite-groups
      x-api-path-slug: usersselffavoritesgroups-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Groups
  /users/self/favorites/groups/{id}:
    delete:
      summary: Remove group from favorites
      description: Remove group from favorites.
      operationId: remove-group-from-favorites
      x-api-path-slug: usersselffavoritesgroupsid-delete
      parameters:
      - in: query
        name: id
        description: the ID or SIS ID of the group to remove
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Groups
      - Id
    post:
      summary: Add group to favorites
      description: Add group to favorites.
      operationId: add-group-to-favorites
      x-api-path-slug: usersselffavoritesgroupsid-post
      parameters:
      - in: query
        name: id
        description: The ID or SIS ID of the group to add
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Groups
      - Id
  /users/self/groups:
    get:
      summary: List your groups
      description: List your groups.
      operationId: list-your-groups
      x-api-path-slug: usersselfgroups-get
      parameters:
      - in: query
        name: context_type
        description: Only include groups that are in this type of context
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Groups
  /users/self/todo:
    get:
      summary: List the TODO items
      description: List the todo items.
      operationId: list-the-todo-items
      x-api-path-slug: usersselftodo-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Todo
  /users/self/upcoming_events:
    get:
      summary: List upcoming assignments, calendar events
      description: List upcoming assignments, calendar events.
      operationId: list-upcoming-assignments-calendar-events
      x-api-path-slug: usersselfupcoming-events-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Upcoming
      - Events
  /users/{id}:
    get:
      summary: Show user details
      description: Show user details.
      operationId: show-user-details
      x-api-path-slug: usersid-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Id
    put:
      summary: Edit a user
      description: Edit a user.
      operationId: edit-a-user
      x-api-path-slug: usersid-put
      parameters:
      - in: query
        name: user[avatar][token]
        description: A unique representation of the avatar record to assign as the
          user&#39;sncurrent avatar
      - in: query
        name: user[avatar][url]
        description: To set the user&#39;s avatar to point to an external url, do
          not include antoken and instead pass the url here
      - in: query
        name: user[email]
        description: The default email address of the user
      - in: query
        name: user[locale]
        description: The user&#39;s preferred language as a two-letter ISO 639-1 code
      - in: query
        name: user[name]
        description: The full name of the user
      - in: query
        name: user[short_name]
        description: User&#39;s name as it will be displayed in discussions, messages,
          andncomments
      - in: query
        name: user[sortable_name]
        description: User&#39;s name as used to sort alphabetically in lists
      - in: query
        name: user[time_zone]
        description: The time zone for the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - Id
  /users/{id}/colors:
    get:
      summary: Get custom colors
      description: Get custom colors.
      operationId: get-custom-colors
      x-api-path-slug: usersidcolors-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Id
      - Colors
  /users/{id}/colors/asset_string:
    get:
      summary: Get custom color
      description: Get custom color.
      operationId: get-custom-color
      x-api-path-slug: usersidcolorsasset-string-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Id
      - Colors
      - Asset
      - String
    put:
      summary: Update custom color
      description: Update custom color.
      operationId: update-custom-color
      x-api-path-slug: usersidcolorsasset-string-put
      parameters:
      - in: query
        name: hexcode
        description: The hexcode of the color to set for the context, if you choose
          to pass thenhexcode as a query parameter rather than in the request body
          you should NOTninclude the &#39;#&#39; unless you escape it first
      responses:
        200:
          description: OK
      tags:
      - Users
      - Id
      - Colors
      - Asset
      - String
  /users/{id}/merge_into/accounts/destination_account_id/users/{destination_user_id}:
    put:
      summary: Merge user into another user
      description: Merge user into another user.
      operationId: merge-user-into-another-user
      x-api-path-slug: usersidmerge-intoaccountsdestination-account-idusersdestination-user-id-put
      responses:
        200:
          description: OK
      tags:
      - Users
      - Id
      - Merge
      - Into
      - Accounts
      - Destination
      - Account
      - Id
      - Users
      - Destination
      - User
      - Id
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