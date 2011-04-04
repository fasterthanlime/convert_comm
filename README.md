# convert_comm

Took me 10 minutes to write, is actually a loosy excuse for a sed program,
converts stuff like this:

    # Retrieve a list of the tracks of this user
    #
    # @param [String] user_id: id or login
    # @param [Integer] limit (50) limit per page
    # @param [Bool] embed (false) should embed codes be included in the response
    # @return [Hashie::Mash] Track list

Into stuff like this:

    /**
     * Retrieve a list of the tracks of this user
     *
     * @param string user_id: id or login
     * @param integer limit (50) limit per page
     * @param bool embed (false) should embed codes be included in the response
     * @return array Track list
     */

## Usage

convert_comm "your ruby doc comment"

Outputs the php style comment to the standard output.

Have fun!
