# SPDX-License-Identifier: AGPL-3.0-or-later
# Copyright (C) 2026 BLT Sandwich

# This program is free software: you can redistribute it and/or modify
# it under the terms of the GNU Affero General Public License as published by
# the Free Software Foundation, either version 3 of the License, or
# (at your option) any later version.

# This program is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU Affero General Public License for more details.

# You should have received a copy of the GNU Affero General Public License
# along with this program.  If not, see <https://www.gnu.org/licenses/>.

project(
  'daemon-utils', 'c',
  version: '1.0.0', meson_version: '>=1.3.0',
  default_options: ['sysconfdir=/etc']
)

cc = meson.get_compiler('c')
includes = include_directories('include')
if get_option('manpages')
  pod2man = find_program('pod2man', required: true)
  subdir('man')
endif
subdir('src')
