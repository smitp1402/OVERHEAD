
  <img src="readme_assets/intro.png" alt="intro" width='100%' height='auto'/>
  <p>
      Overhead is a rudimentary game engine, made using Java SE8, LWJGL (Light Weight Java Gaming Library) and JOML (Java OpenGL Math Library). 
      It is equipped with:
      <ol>
        <li>
          an entity system
        </li>
        <li>
          an animation system
        </li>
        <li>
          a collision system
        </li>
        <li>
          a tileset system
        </li>
        <li>
          a texture system
        </li>
        <li>
          a world
        </li>
        <li>
          an input handler
        </li>
        <li>
          a camera
        </li>
        <li>
          shaders
        </li>
        <li>
          a screen tile renderer
        </li>
     </ol>  
  </p>
  <a href='https://www.youtube.com/watch?v=oxdO2_ccgTQ'>Trailer</a>
  
  
  
  <h1> Gallery </h1>
  <h3> This is a gallery for Overhead: The Game (a small game made in Overhead: The Engine) </h3>
  
  <h6>
      Overhead: The game is a short maze. The player has to navigate through it. 
      <br />
      The sole purpose of this game is to test the functionalities of the Engine.
  </h6>
  
  <br /><br />
  <p>
      1. An independent window is initialised. For those familiar with Windows forms, this is a classic SDI Win-form.
  </p>
  <img align='center' src='readme_assets\story_1.png' alt="story_1" width='70%' height='auto'/>
  
  <p>
      2.The player is an entity. It has its anims set by the animation system, which has the options to add new anims (this example only has an idle and running animation). It           also has a collidable.
      <br />
      3. Input is handled by the Input.java class. It too can be customised for additional input events.
      <br />
      4. An entity for the floor is also present. It does not have a collidable attached, so the player can walk on it.
  </p>
  <img align='center' src='readme_assets\story_4.gif' alt="story_4" width='70%' height='auto'/>
  
  <p>
      5.There is an entity for the walls, with its collidable. The player and the walls are in the same collision layer, and hence they collide.
      <br />
      6. The collidable work through the concept of Axis Aligned Bounding Boxes (AABB).
  </p>
  <img align='center' src='readme_assets\story_3.gif' alt="story_3" width='70%' height='auto'/>
  
  <p>
      7. A camera is also initialised. It is made to follow the player, with smoothness. There is also a 'blind region', wherein if player moves, the camera will not budge.
      <br />
      8. There are also bounds to the world, inside which the camera is wrapped. That is, if the player reaches the edges of the world, the camera stops moving.
  </p>
  <img align='center' src='readme_assets\story_2.gif' alt="story_2" width='70%' height='auto'/>
  
  <p>
      8. The viewport (area visible inside the camera) is the only place where the textures are rendered. Everywhere outside the camera is not rendered. This is an attempt at            hyper-efficiency for the largest of in-game worlds.
  </p>
  <img align='center' src='readme_assets\story_5.gif' alt="story_5" width='70%' height='auto'/>
  
  <p>
      9. The renderer, animations, and basically everything that needs work frame-by-frame works at the same refresh-rate. This is set up using pretty standard timer and                  interval logic. Here, it is capped at 60 fps (customisable).
  </p>
  <img align='center' src='readme_assets\story_6.png' alt="story_6" width='auto' height='70%'/>
  
  
  
  <h1> Prerequisites </h1>
  <ul>
      <li>
        <a href='https://www.oracle.com/in/java/technologies/javase/javase-jdk8-downloads.html'> Java SE8 SDK </a>
      </li>
      <li>
        <a href='https://www.eclipse.org/downloads/packages/release/kepler/sr1/eclipse-ide-java-developers'> Eclipse IDE for Java </a>
      </li>
      <li>
        <a href='https://www.lwjgl.org/download'> LWJGL </a>
      </li>
      <li>
        <a href='https://jar-download.com/?search_box=joml'> JOML </a>
      </li>
  </ul>
  
  
  
  <h1> Getting Started </h1>
  <p>
      1. Start up the engine (run the exe file, which in my case is Godot_v3.2.1-stable_win64.exe)
  </p>

  <p>
      2. Select the 'Import' option 
  </p>
  <img align='center' src='readme_assets\getting_started_1.png' alt="getting_started_1" width='80%' height='auto'/>
    
  <p>
      3. Browse to where the project has been downloaded
  </p>
    
  <p>
      4. Select the 'project.godot' file, and open it
  </p>
  <img align='center' src='readme_assets\getting_started_2.png' alt="getting_started_2" width='80%' height='auto'/>
    
  <p>
      5. Press the 'Play' button in the top right
  </p>
  <img align='center' src='readme_assets\getting_started_3.png' alt="getting_started_3" width='80%' height='auto'/>
    
  <p>
      Enjoy! <a href='https://www.eclipse.org/getting_started/'>Operating through Eclipse</a> is a breeze.
  </p>
  
  
  
  <h1> Deployment </h1>
  <p>
      There is no implementation for a sophisticated deployment system. 
      <br /> 
      One can pack and encrypt all files in order except the Overhead.java file, to make it a faux-deployed application.
  </p>
   
   
   
  <h1> Built with </h1>
  <ul>
      <li>
        <a href='https://www.eclipse.org/downloads/packages/release/kepler/sr1/eclipse-ide-java-developers'> Eclipse IDE for Java </a>
      </li>
      <li>
        <a href='https://www.lwjgl.org/download'> LWJGL </a>
      </li>
      <li>
        <a href='https://jar-download.com/?search_box=joml'> JOML </a>
      </li>
  </ul>
   
   
   
  <h1> Co-authors </h1>
  <p>
      <a href='https://github.com/smitp1402'> Smit Panchal </a>
      <br/>
      <a href='https://github.com/edgeemperor'> Sanpreet Singh Gill </a>
  </p>
   
   
   
  <h1> Acknowledgments </h1>
  <p>
      Taught completely by the YouTube course <a href='https://www.youtube.com/watch?v=VH9KAhjXVFM&list=PLILiqflMilIxta2xKk2EftiRHD4nQGW0u'>game development in LWJGL by Warmful       Development</a>.
  </p>
