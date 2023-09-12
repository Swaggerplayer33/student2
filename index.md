<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Random Background with Descriptions</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            /* Set initial background image or color */
            background: url('initial-background.jpg') no-repeat center center fixed;
            background-size: cover;
        }
        #description {
            position: absolute;
            top: 10px;
            left: 10px;
            color: white; /* Set text color to white */
            background-color: rgba(0, 0, 0, 0.5);
            padding: 5px;
            border-radius: 5px;
        }
    </style>
</head>
<body>
<hr>
<h1 id="-u-font-size-100px-style-color-blue-tanav-s-page-font-u-"><strong><u><font size=100px style="color:blue">~Tanav&#39;s Page~</font></u></strong></h1>
<p>Go to my <a href="https://github.com/Swaggerplayer33">Github account</a></p>
<hr>
<h2 id="-strong-style-color-blue-here-is-my-freeform-image-strong-"><strong  style="color:blue">  Here is my freeform image!</strong></h2>
<p><img src="images/ink.png" alt="Freeform" title="Freeform drawing, this image shows my interests, which include basketball, cad, coding, and my ethnicity"></p>
<font size = 25px style="color:blue">Here are some fun facts about me!</font>


<table>
<thead>
<tr>
<th>1. I enjoy playing basketball with my friends</th>
<th>2. I like to play the piano</th>
</tr>
</thead>
<tbody>
<tr>
<td>3. My favorite food is pizza</td>
<td>4. My favorite animals are birds</td>
</tr>
<tr>
</tr>
<tr>
<td>5. I was born in India</td>
<td>6. In my free time I play video games</td>
</tr>
</tbody>
</table>
<h2 id="-strong-style-color-blue-i-love-spending-time-in-nature-strong-"><strong style="color:blue">  I love spending time in nature!</strong></h2>
<p><img src="images/nature_image.jpeg" alt="Nature" title="Nature image"></p>
<hr>
<h2 id="-span-style-color-red-overview-of-hacks-study-and-tangibles-span-"><span style="color:red">Overview of Hacks, Study and Tangibles</span></h2>
<p>Blogging in GitHub pages is a way to learn and code at the same time. </p>
<ul>
<li>Plans, Lists, <a href="https://clickup.com/blog/scrum-board/">Scrum Boards</a> help you to track key events, show progress and record time.  Effort is a big part of your class grade.  Show plans and time spent!</li>
<li><a href="https://levelup.gitconnected.com/six-ultimate-daily-hacks-for-every-programmer-60f5f10feae">Hacks(Todo)</a> enable you to stay in focus with key requirements of the class.  Each Hack will produce Tangibles.</li>
<li>Tangibles or <a href="https://en.wikipedia.org/wiki/Artifact_(software_development">Tangible Artifacts</a>) are things you accumulate as a learner and coder. </li>
</ul>
   <div id="description"></div>
    <script>
        // Define an array of background image URLs and their descriptions
        const backgrounds = [
            {
                url: 'https://assets3.cbsnewsstatic.com/hub/i/r/2021/08/02/ad96efb4-2405-4b26-a093-41993790fc6c/thumbnail/640x637/166bb875d83de6a901c48b798342d0e8/eaglenebula.jpg?v=181d27d1e918a6408b48ea2e220df310',
                description: 'These are the pillars of creation, found deep in the Eagle nebula',
            },
            {
                url: 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS3fSb1i3y_a1WGSsRcpCllRJhsYDU3w0RNJw&usqp=CAU',
                description: 'This is the Rho Ophiuchi nebula, a home to millions of baby stars',
            },
            {
                url: 'https://sm.mashable.com/t/mashable_in/photo/default/crab-nebula-mosaic_pvft.720.jpg',
                description: 'This is the crab nebula',
            },
            {
                url: 'https://media.cnn.com/api/v1/images/stellar/prod/230907143646-spacex-starship.jpg?c=16x9&q=h_720,w_1280,c_fill',
                description: 'This is the SpaceX starship, my favorite rocket. Its mission is to land on Mars',
            },
            // Add more image URLs and descriptions as needed
        ];

        // Function to set a random background image and description
        function setRandomBackground() {
            const randomIndex = Math.floor(Math.random() * backgrounds.length);
            const randomBackground = backgrounds[randomIndex];
            document.body.style.backgroundImage = `url('${randomBackground.url}')`;
            const descriptionElement = document.getElementById('description');
            descriptionElement.textContent = randomBackground.description;
            descriptionElement.style.color = 'white'; // Set text color to white
        }

        // Call the function to set a random background and description when the page loads
        window.addEventListener('load', setRandomBackground);
    </script>
</body>
</html>



