# Quick Start
Check the [quick start](https://github.com/can-can/TypeeChromeExtensionDoc/blob/main/docs/quick-start.md) First

# What is Typee Chrome Extension

Typee Browser Extension is keyboard first productivity tool that helps you interact with browser faster and more
efficiently.

## Installation

https://chromewebstore.google.com/detail/typee-a-browser-command-l/agifbaonnnpmdpnemfhddffdledhhnen

## How to Use

By typing keys Control + J on any page, Typee shows a command line and list of commands.

Choose a command you want.

# Features

## Various Commands

the commands are categorized as below

#### Tab Management

#### Tab Group Management

#### Typee Settings

#### Site Specific Commands

Currently it support twitter

#### Alias Management

#### Expansion Management

#### Content Copy

#### Click on Page

## Alias

The fundamental commands usually have multiples options. it is not convenient to fill out the options.

You can create a alias by adding alias option when you executing a command

## Expansion

Expansion is similar to alias but creates alias automatically with definition.
Below configuration will create alias going to tabs directly. The count of alias depends on current tabs.

```
{
      "shortcutId": "goToTab",
      "expandedOptionName": "target",
      "nameOptions": {
        "prefix": "Go To Tab |",
        "ignoreExtendedOptionsNames": true
      }
}
    
```

If you want to add this configuration, please choose `expansion` command and `add` option, the value should be in one
line `{"shortcutId": "goToTab","expandedOptionName": "target","nameOptions": {"prefix": "Go To Tab |","ignoreExtendedOptionsNames": true}}`

### All Shared Expansion Configs
#### Go To Tab
`{"shortcutId": "goToTab","expandedOptionName": "target","nameOptions": {"prefix": "Go To Tab |","ignoreExtendedOptionsNames": true}}`
#### Move Current Tab to a Group
`{"shortcutId": "moveTab","expandedOptionName": "tabGroup","nameOptions": {"prefix": "Move Current Tab to Group |","ignoreExtendedOptionsNames": true}}`
#### Expand Tab Group
`{"shortcutId": "expandTabGroup","expandedOptionName": "target","nameOptions": {"prefix": "Expand Tab Group |","ignoreExtendedOptionsNames": true}}`
#### Collapse Tab Group
`{"shortcutId": "collapseTabGroup","expandedOptionName": "target","nameOptions": {"prefix": "Collapse Tab Group |","ignoreExtendedOptionsNames": true}}`
