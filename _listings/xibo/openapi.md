swagger: "2.0"
x-collection-name: Xibo
x-complete: 1
info:
  title: Xibo API
  description: xibo-cms-api
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /playlist/widget/audio/{playlistId}:
    post:
      summary: Parameters for editing existing audio widget on a layout
      description: Parameters for editing existing audio widget on a layout, for adding
        new audio, please refer to POST /library documentation
      operationId: WidgetAudioEdit
      x-api-path-slug: playlistwidgetaudioplaylistid-post
      parameters:
      - in: formData
        name: duration
        description: Edit Only - The Widget Duration
      - in: formData
        name: loop
        description: Edit only - Flag (0, 1) Should the audio loop (only for duration
          > 0 )?
      - in: formData
        name: mute
        description: Edit only - Flag (0, 1) Should the audio be muted?
      - in: formData
        name: name
        description: Edit Only - The Widget name
      - in: formData
        name: useDuration
        description: Edit Only - (0, 1) Select 1 only if you will provide duration
          parameter as well
      responses:
        200:
          description: OK
      tags:
      - Parametersediting
      - Existing
      - Audio
      - Widget
      - "On"
      - Layout
  /playlist/widget/image/{playlistId}:
    post:
      summary: Parameters for editing existing image on a layout
      description: Parameters for editing existing image on a layout, for adding new
        images, please refer to POST /library documentation
      operationId: WidgetImageEdit
      x-api-path-slug: playlistwidgetimageplaylistid-post
      parameters:
      - in: formData
        name: alignId
        description: Edit only - Horizontal alignment - left, center, bottom
      - in: formData
        name: duration
        description: Edit Only - The Widget Duration
      - in: formData
        name: name
        description: Edit only - Optional Widget Name
      - in: formData
        name: scaleTypeId
        description: 'Edit only - Select scale type available options: center, stretch'
      - in: formData
        name: useDuration
        description: Edit only (0, 1) Select 1 only if you will provide duration parameter
          as well
      - in: formData
        name: valignId
        description: Edit only - Vertical alignment - top, middle, bottom
      responses:
        200:
          description: OK
      tags:
      - Parametersediting
      - Existing
      - Image
      - "On"
      - Layout
  /playlist/widget/pdf/{playlistId}:
    post:
      summary: Parameters for editing existing pdf on a layout
      description: Parameters for editing existing pdf on a layout, for adding new
        files, please refer to POST /library documentation
      operationId: WidgetPdfEdit
      x-api-path-slug: playlistwidgetpdfplaylistid-post
      parameters:
      - in: formData
        name: duration
        description: Edit Only - The Widget Duration
      - in: formData
        name: name
        description: Edit only - Optional Widget Name
      - in: formData
        name: useDuration
        description: (0, 1) Select 1 only if you will provide duration parameter as
          well
      responses:
        200:
          description: OK
      tags:
      - Parametersediting
      - Existing
      - Pdf
      - "On"
      - Layout
  /playlist/widget/video/{playlistId}:
    post:
      summary: Parameters for editing existing video on a layout
      description: Parameters for editing existing video on a layout, for adding new
        videos, please refer to POST /library documentation
      operationId: WidgetVideoEdit
      x-api-path-slug: playlistwidgetvideoplaylistid-post
      parameters:
      - in: formData
        name: duration
        description: Edit Only - The Widget Duration
      - in: formData
        name: loop
        description: Edit only - Flag (0, 1) Should the video loop (only for duration
          > 0 )?
      - in: formData
        name: mute
        description: Edit only - Flag (0, 1) Should the video be muted?
      - in: formData
        name: name
        description: Edit only - Optional Widget Name
      - in: formData
        name: scaleTypeId
        description: 'How should the video be scaled, available options: aspect, stretch'
      - in: formData
        name: useDuration
        description: Edit Only - (0, 1) Select 1 only if you will provide duration
          parameter as well
      responses:
        200:
          description: OK
      tags:
      - Parametersediting
      - Existing
      - Video
      - "On"
      - Layout
  /playlist/widget/{widgetId}/audio:
    put:
      summary: Parameters for edting/adding audio file to a specific widget
      description: Parameters for edting/adding audio file to a specific widget
      operationId: WidgetAssignedAudioEdit
      x-api-path-slug: playlistwidgetwidgetidaudio-put
      parameters:
      - in: formData
        name: loop
        description: Flag (0, 1) Should the audio loop if it finishes before the widget
          has finished?
      - in: formData
        name: mediaId
        description: Id of a audio file in CMS library you wish to add to a widget
      - in: formData
        name: volume
        description: Volume percentage(0-100) for this audio to play at
      - in: path
        name: widgetId
        description: Id of a widget to which you want to add audio or edit existing
          audio
      responses:
        200:
          description: OK
      tags:
      - Parametersedting
      - Adding
      - Audio
      - File
      - To
      - Specific
      - Widget