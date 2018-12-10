To customize the game, follow the instructions on the CustomizeGameHere event sheet.

The remaining information in this file is further documentation into how the template works in case you want to extend or enhance the game engine.

1.  Each physical copy of the Image sprite on the SoundBoard has a zero-based Position instance variable that uniquely identifies it. This value is used along with modulo and ceiling functions to provide for pagination.

2.  If there are fewer Animation Frame images than slots on the board (6 by default), the last image available will be replicated for all the remaining slots when editing the SoundBoard layout. This occurs because Construct 2 does not allow an invalid value for the Initial Frame of an animation. At runtime the replication will not appear (due to an explicit test in the script), and the application will behave correctly.

3. A navigation option to return to the StartScreen is provided (ShowHomeButton) but turned off by default, since currently there's no need return to the StartScreen once you are playing the game.