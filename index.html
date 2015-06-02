<!doctype html> 
<html lang="en"> 
<head> 
	<meta charset="UTF-8" />
    <title>Felipão - Uma aventura no México</title>
	<script type="text/javascript" src="js/phaser.min.js"></script>
    <style type="text/css">
        body {
            margin: 0;
        }
    </style>
</head>
<body>

<script type="text/javascript">
var game = new Phaser.Game(800, 600, Phaser.AUTO, '', { preload: preload, create: create, update: update });

function preload() {

    game.load.image('bg', 'assets/bg.jpg');
    game.load.image('ground', 'assets/platform.jpg');
    game.load.image('fireworks', 'assets/fireworks.png');
    game.load.spritesheet('felipao', 'assets/sprite-felipao-s.png', 153, 220);
    game.load.audio('boden', ['assets/hahaha.mp3']);

}

var player;
var platforms;
var cursors;
var title;
var score=0;
var music;

function create() {

    game.physics.startSystem(Phaser.Physics.ARCADE);

    game.add.sprite(0, 0, 'bg');

    platforms = game.add.group();

    platforms.enableBody = true;

    var ground = platforms.create(0, game.world.height - 44, 'ground');

    ground.scale.setTo(2, 2);

    ground.body.immovable = true;

    player = game.add.sprite(0, 50, 'felipao');

    game.physics.arcade.enable(player);

    player.body.bounce.y = 0.1;
    player.body.gravity.y = 800;
    player.body.collideWorldBounds = true;

    player.animations.add('left', [5, 6, 7, 8], 10, true);
    player.animations.add('right', [1, 2, 3, 4], 10, true);

    fireworks = game.add.group();

    fireworks.enableBody = true;

    for (var i = 1; i < 4; i++)
    {
        var firework = fireworks.create(i * 200, 0, 'fireworks');

        firework.body.gravity.y = 500;

        firework.body.bounce.y = 0.3 + Math.random() * 0.2;
    }

    title = game.add.text(16, 16, 'Felipão - Uma aventura no México', { fontSize: '32px', fill: '#fff' });

    cursors = game.input.keyboard.createCursorKeys();
}

function update() {

    game.physics.arcade.collide(player, platforms);
    game.physics.arcade.collide(fireworks, platforms);

    game.physics.arcade.overlap(player, fireworks, collect, null, this);

    player.body.velocity.x = 0;

    if (cursors.left.isDown)
    {
        player.body.velocity.x = -150;

        player.animations.play('left');
    }
    else if (cursors.right.isDown)
    {
        player.body.velocity.x = 150;

        player.animations.play('right');
    }
    else
    {
        player.animations.stop();

        player.frame = 0;
    }
    
    if (cursors.up.isDown && player.body.touching.down)
    {
        player.body.velocity.y = -350;
    }

}

function collect (player, firework) {

    firework.kill();
    score++;

    if (score==3) {
        var scoreText = game.add.text(300, 200, 'HAHAHAHAHAHAHA', { fontSize: '32px', fill: '#fff' });
        music = game.sound.play('boden');
    };

}


</script>

</body>
</html>