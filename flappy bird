const config ={
    width: 825,
    height: 550,
    type : Phaser.AUTO,
    physics: {
        default: 'arcade',
        arcade: {
            gravity: {y: 525}
        }
    },
    scene: {
        preload: preload,
        create: create,
        update: update,
    }
}

var game = new Phaser.Game(config)
let dude
let cursors

function preload() {
    this.load.image('dude', 'img/oiseau.png')
    this.load.image('fond2.png', 'img/fond2.png')
}

function create() {

    
    this.add.image(300,150, 'fond2.png'),

    dude = this.physics.add.image(300, 300, 'dude')
    dude.setScale(1/5,1/5 )
    dude.body.setSize(100, 200);
    dude.setCollideWorldBounds(true);
    cursors = this.input.keyboard.createCursorKeys()
    console.log(cursors)
}

function update(){
    dude.setVelocityX(0)

    if(cursors.up.isDown)
        dude.setVelocity(0, -300)


}
