# Boards

The Boards Action Item lets you both add a request to one or more boards within the Board Manager app and view which boards the request is currently on.

## Adding a request to a Board

From the drop-down select the board and list you wish to add the request to.

* The list of Boards displayed will be filtered to those that the viewing analyst has the right to view and add to.

## Viewing the Boards a request is already present on

Once the request has been added to one or multiple Boards, either manually from the request or through workflow automation, the boards the request is on will be visible.

* You can click on the board, to be taken directly to the board to view the request on the board

## Removing a request from a Board

Each Board listed in the Boards action item provides an X which when selected the request that you are currently viewing will be removed from that board. This option is not available to users that Read Only access to a board.

## Advanced setting

A [Service Manager application setting](/servicemanager-config/advanced-tools-and-settings/application-settings) is available that will automatically remove a request from all associated boards if the request status is set to canceled.

* `autoremove.canceled.request.from.boards`

:::note
This setting will not be applied to any request that was raised prior to this setting being [available](https://community.hornbill.com/topic/29556-new-update-service-manager-3470/).
:::
