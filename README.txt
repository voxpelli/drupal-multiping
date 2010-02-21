Multiping is a replacement for the old ping module of the core distribution.

Features:
- configure multiple ping services via web interface
- ping via XMLRPC or specially formatted URL
- select ping services depending on taxonomy values of a node
  (e.g. have a taxonomy for the language of a node and ping German
  ping services only for German articles; or:
  ping certain technical oriented ping services only if a node is
  assigned to certain technical taxonomy terms)
- ping during cron runs or immediately after node submission
- if a ping service cannot be reached, the ping is retried in exponentially
  increasing intervals to avoid "hammering" the service.

Changes in behaviour comparing to the core module:
- No longer uses the ping hook (no ping events are generated)

Credits:
Thanks to all bug reporters (and sorry for any long delays).
Thanks to John Morahan for the patch correcting the watchdog calls.


This program is free software; you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation; version 2 of the License.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

