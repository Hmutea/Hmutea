//Credit By MZO BOT
const chalk = require("chalk")
const fs = require("fs")

//aumto presence update
global.AntiCallBot = false // false a i dah chuan, rawn call-tu che automatic a block a ni lovang
global.GroupWcMsg = true // false a i dah chuan welcome message i off ang
global.autoTyping = false // true a i dah chuan i type la a lang ang
global.autoRecord = false // true a i dah chuan Voice record angin i lang ang
global.available = true // false a i dah chuan offline angin a awm ang
global.public = true // false ah i dah chuan nang chauhin i hmang thei ang
global.autoread = false // true a i dah chuan message zawng zawng read vek zelin a awm ang 
global.autoread_status = false // true a i dah chuan auto status view in a awm ang
global.default_language = true // default language i hman dawn loh chuan false ah hia  dah tur
global.mtl_language = false // multi language i hman dawn chuan true ah dah tur
global.bot_language = 'lus' // I language code dah tur code hman i hriat loh chuan https://herbert70.blogspot.com/p/language-code-for-hbwabot.html?m=1 he link ah hian en thei a ni ang

//info
global.owner = ['918837094883'] // I phone number in thlak rawh
global.ownernumber = '918837094883' // I phone number in thlak rawh
global.ownername = "꧁HKIMA42♕꧂" // I hming dah tel bawk la
global.location = "India, Mizoram, Khawzawl vegthar" // I awmna hmun daha
global.botname = "HKIMA_42" // I bot hming tur dah la
global.ownerweb = "https://youtube.com/@HBMods_Channel"
global.themeemoji = '🌚'
global.creator = "918837094883@s.whatsapp.net" // @ symbol hmaa number hi i phone number in thlak rawh

global.ownerNumber = ["918837094883@s.whatsapp.net"]// @ symbol hmaa number hi i phone number in thlak rawh
global.prefa = ['','!','.','#','/']
global.sessionName = 'session'

// Sticker Pack Name
global.packname = "Sticker ByHKIMA_42"
global.author = "HKIMA_42"

//BUTTON INPUT 
global.buttonyt = "SUBSCRIBE"
global.buttonyturl = "https://youtube.com/@h.kima44?si=Nh3nTgYx0hvNb2Vb "
global.buttonig = "Follow Us:)"
global.buttonigurl = "https://www.instagram.com/hkima_42?igsh=czNrbnptOG5odHR3"
//_______________________________________________
global.defaultpp = 'https://cdn.pixabay.com/photo/2015/10/05/22/37/blank-profile-picture-973460_960_720.png?q=60'
//messages
global.mess = {
    success: '\n*©HKIMA_42*!', 
    admin: 'He features hi chu admin-te chauh hman thei tur a siam a ni!',
    botAdmin: 'Admin-ah min dah hmasa phawt la chuan ka ti thei ang!',
    owner: 'He features hi a neitu chauh hman thei tura siam a ni!',
    group: 'Hei chu group-ah chauh hman thei tura siam a ni!',
    private: 'Hei chu private chat-ah chauh hman thei tura siam a ni!',
    bot: 'Hei chu kei mah chauh hman thei tur a siam a ni',
}

let file = require.resolve(__filename)
fs.watchFile(file, () => {
	fs.unwatchFile(file)
	console.log(chalk.redBright(`Update'${__filename}'`))
	delete require.cache[file]
	require(file)
})
