This is a simple toolkit for creating LightNCandy-based skins for MediaWiki.

To create a LightNCandy-based skin, you do the following:

1. Create your template class, just make a class that derives from LightNCandyTemplate,
   and override the getTemplate() method to return a LightNCandy template method.
   The easiest way to implement this is to use my
   [simple-lightncandy](https://github.com/werdnum/simple-lightncandy) class and call
   its getTemplate() method.
2. Create your skin class. Derive from SkinTemplate and set its $template member variable
   to the class name of your template class.
3. Register your skin with the factory.

For a full example, see [LivingStyleGuideSkin](https://github.com/werdnum/LivingStyleGuideSkin).
