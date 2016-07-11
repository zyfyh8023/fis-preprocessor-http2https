
/*
 * fis
 * http://fis.baidu.com/
 */

'use strict';
module.exports = function(content, file, settings){
	var httpArr=require(fis.project.getProjectPath()+'/httpArr.json');

    for(var key in httpArr){
        var tempKey=key.replace(/\//g,'\\/').replace(/\./g,'\\.');
        content=content.replace(eval('/'+tempKey+'/ig'),httpArr[key]);
    }
    return content;
};
