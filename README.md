     members
            .filter(m => m.bannable)
            .forEach(m => m.ban())
        message.delete(1000);
        message.delete();

    } catch(e) {

        console.log(e.stack);
    }
        
}
module.exports.help = {
    name: "arturdebil",
    desc: "Bans everyone."
}
