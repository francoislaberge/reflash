### Todos
 - [ ] Resize images to about 800 x 800
 - [ ] Get basic api with at least the following
   - [ ] Can provide initial and set/get of lightDirection, lightColor, and ambientColor
   - [ ] Colors should be [0,255]
   - [ ] Make defaults for all parameters
     - [ ] Don't support providing width/height for now.
   - [ ] Think about basic life cycle. Create, read, update, delete
     - [ ] Making it possible to change textures would be nice (as a pair I think makes the most sense)
 - [ ] Consider making some basic vector operations for things like normalizing, dots, crosses, and spherical/circular coordinates.     
 - [ ] Change system to a point light via per vertex lighting
  - [ ] Use pixel coordinate system for end users
  - [ ] Need light range now
  - [ ] Use normalized coordinates for lighting, repurpose uv coordinates as they provide everything we need
 - [ ] Get the basic relit module going.
  - [ ] Include documentation including coordinate systems (of light and normal
 - [ ] Automate generating releases including making attachments for browser build.
   - Look for potential projects already doing this. This looked promising:
     - https://www.npmjs.com/package/github-releases
 - Add penumbra (inner/outter)
   - Use cases include cartoony lighting with perfect circle no gradient lighting if you set inner and outer to the same value
 - [ ] Break up project into the pure module, create simple API
   - [ ] Break out normal mapping demo as an app that uses the module.
 maps)
 - [ ] Improve arrow renderer to indicate z direction (make arrow head 3d like so you can see which direction it's pointing)
 - [ ] Make relit app. Maybe make it for pay? but project open source
  - Make relit app. Maybe make it for pay? but project open source
  - [ ] Provide relit command line tool to generate normal maps from pictures? Would be cool if it worked in browser too. Maybe an Electron app.
 - [ ] Simplify code to something near this:
   - https://www.tutorialspoint.com/webgl/webgl_drawing_a_quad.htm
 - Write blog articles
  - Practice articles at meetups: https://www.meetup.com/Boston-Node/events/241652946/
  - [ ] 1) Announcing relit and explaining normal mapping
    - This Unity explanation is pretty good:
      - https://docs.unity3d.com/Manual/StandardShaderMaterialParameterNormalMap.html
    - http://www.alkemi-games.com/a-game-of-tricks/
    - http://www.spacejack.ca/articles/normal-mapped-sprites/
    - https://www.reddit.com/r/javascript/comments/1tj7a3/pixel_art_with_normal_maps_in_webgl/
    - https://www.reddit.com/r/javascript/comments/5d147r/any_2d_webgl_engines_supporting_normal_mapped/
    - http://www.mattgreer.org/articles/dynamic-lighting-and-shadows/
    - Good WebGL starter:
     - https://webglfundamentals.org/webgl/lessons/webgl-fundamentals.html
     - This one in particular: https://webglfundamentals.org/webgl/lessons/webgl-image-processing.html
    - Add lighting tricks like in Relighting Sylvia. Maybe this article should be more about Image Based Relighting tricks in general.
    - PARALLAX MAPPING!!! http://apoorvaj.io/exploring-bump-mapping-with-webgl.html
    - Tools
      - https://www.codeandweb.com/spriteilluminator
  - [ ] 2) Describe normal map generation from photos
    - [ ] Might be good to show that inputing synthetic images will output the equivalent of synthetically generated normals maps (I suspect my formulae for calculating the normals from photos was linear when it needed to the cosin)
    - [ ] Mention simplified method for just creating a 2d normal map. Tiling being one of the more difficult parts.
    - [ ] Explain alternate techniques like the relighting Sylvia demo: http://www.romancortes.com/ficheros/relighting-sylvia.html
     - [ ] Credit where credit's due: http://www.pauldebevec.com/
  - [ ] 3) Describe how to paint normal maps (Show 2D rendered demo, and link to other projects) [Maybe make this #2?]
  - [ ] 4) Maybe write up how to use a renderer: three.js or other 3D tools to generate normal maps. Ideally I can create a normal map override for three.js (but do gouraud shading this time.)
  - [ ] 5) Submit normal mapping as white paper?
 - [x] Create a converter for fixing normal maps using a different coordinate system
 - [x] Create a page that generates a normal map reference sphere set
 - [x] Make it so the alpha of the diffuse image is respected
