#Pygmynote

Pygmynote is a command-line tool for storing and managing heterogeneous bit of data like notes, tasks, links, file attachments, etc. Pygmynote is written in Python and uses an SQLite database as its back end.

##Features

- Add, update, archive, and delete records
- Specify dates for records to turn them into tasks
- Add long notes using an external text editor
- Add records with attachments
- Search records by note and by tag
- View active and archived records
- Run user-defined SQL queries
- Pin and unpin records
- Export records in the TSV format (tab-separated)
- Backup the database
- Generate an HTML file with records containing a specified tag

##Dependencies

- Python 2.x or 3.x
- nano or any other text editor

##Installation

Clone the repository using the `git clone https://github.com/dmpop/pygmynote.git` command. Alternatively, download the provided *zip* or *tar* archive. By default, Pygmynote is configured to use the nano text editor, but you can change that by changing the *EDITOR* variable in the script. To specify a different backup directory, edit the *BACKUP* variable.

##Usage

Open terminal, switch to the *pygmynote* directory and run the _pygmynote.py_ script in the terminal. Type *help* and press `Enter` to list the available commands.

##Localization

	cd pygmynote
	xgettext --language=Python --keyword=_ --output=pygmynote.pot pygmynote.py
	mkdir -p locale/xx/LC_MESSAGES
	cp pygmynote.pot locale/xx/LC_MESSAGES/pygmynote.po
	cd locale/xx/LC_MESSAGES
	msgfmt pygmynote.po -o pygmynote.mo

	$ LANGUAGE=xx python pygmynote.py

##License

This program is free software; you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation; either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with this program; if not, write to the Free Software Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston,MA 02110-1301, USA.

_Copyleft 2010-2016 Dmitri Popov_

Source code: [https://github.com/dmpop/pygmynote](https://github.com/dmpop/pygmynote)
