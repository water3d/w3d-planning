name: User Story
description: An item that relates a user to functionality in the applications
title: "[Story]: "
labels: ["story"]
projects: ["water3d/7"]
body:
  - type: markdown
    attributes:
      value: |
        Please fill in the following information about the use case/user story
  - type: textarea
    id: description
    attributes:
      label: Description
      description: A general overview of the user story
    validations:
      required: true
  - type: input
    id: user-type
    attributes:
      label: User Type
      description: Who is the user this story refers to? (e.g. Growers, Water Managers, but be specific)
      placeholder: Growers
    validations:
      required: true
- type: dropdown
    id: region
    attributes:
      label: Region this supports
      multiple: true
      description: What region does this functionality refer to
      options:
        - Any
        - Western US
        - California
        - San Joaquin Valley
        - New Mexico
        - Mesilla Valley
        - Utah
        - Cache Valley
        - Somewhere Else (please describe)
    validations:
      required: true
  - type: textarea
    id: users-needs
    attributes:
      label: What are this user's needs? What questions do they come to Water3D to answer?
  - type: textarea
    id: success-description
    attributes:
      label: What does success look like for this user? What tools do they use or what information do they leave the application with
  - type: textarea
    id: data-display
    attributes:
      label: Do we have a sense for how this user/story should display data or information?
  - type: textarea
    id: unknowns
    attributes:
      label: What are our unknowns? What additional information do we need before we can consider planning for this story complete?
  - type: textarea
    id: existing-tools
    attributes:
      label: Do existing tools provide any of this functionality? What purpose will it serve to include in Water3D?
  - type: dropdown
    id: time-estimate
    attributes:
      label: Coarse Time Estimate
      description: How long do you think this feature will take to develop
      options:
        - Small (<1 Day)
        - Medium (<1 Week)
        - Large (<1 Month)
        - Significant (>1 Month)
        - Unknown
