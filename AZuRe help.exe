import os
import sys
try:
	import progressbar
except ImportError:
	print '[-] Failed to import progressbar .'
	print '    Run "pip install progressbar2" or "easy_install progressbar2" '
	print 'Use python2 to run this code '
	sys.exit(1)

import urllib2

logo="""
   ______                          _ __        ____        __
  / ____/___  ____ ___  ____ ___  (_) /_      / __ )____  / /_
 / /   / __ \/ __ `__ \/ __ `__ \/ / __/_____/ __  / __ \/ __/
/ /___/ /_/ / / / / / / / / / / / / /_/_____/ /_/ / /_/ / /_
\____/\____/_/ /_/ /_/_/ /_/ /_/_/\__/     /_____/\____/\__/
	"""
while(True):
	os.system('clear')
	print logo
	print "\n\t\tCREATED BY SPEEDX!!!"
	print "\n\n1 - Start BOT "
	print "2 - How To USE"
	print "3 - Exit"
	inp=raw_input('Enter OPTION > ')
	if not inp.find('1')==-1:
		url='https://www.google.com'
		try:
			urllib2.urlopen(url)
		except:
			print 'You Are Not Connected To Internet!!!\nPlease Connect To Internet To Continue....'
			print 'For Any Queries Join Me On WhatsApp!!!'
			print '\t    Group Link: http://bit.do/speedxgit'
			print '\n             Mail: ggspeedx29@gmail.com'
			print '\n  YouTube Channel: https://www.youtube.com/c/GyanaTech'
			sys.exit(2)
		nc=input('Enter Number Of Commits To Do: ')
		gu=raw_input('Enter FULL Git Repository URL(including https://) : ')
		gn=raw_input('Enter Your Github UserName: ')
		ge=raw_input('Enter Your Github E-Mail: ')
		if nc <= 1:
			print '[!] Error Please Enter Number of Commits Greater Than 1 ...'
			raw_input('Press Enter To Continue...')
			continue
		if not gu.startswith('https'):
			print '\n\nALWAYS ENTER FULL REPOSITORY URL\n\tExample: https://github.com/TheSpeedX/commit-bot'
			raw_input('\n\nPress Enter To Continue...')
			continue
		if gu.endswith('.git'):
			gu=gu[0:len(gu)-4]
		if not urllib2.urlopen(gu).code == 200:
			print '[!] Wrong Repository URL !!!'
			print '\n\nALWAYS ENTER FULL REPOSITORY URL\n\tExample: https://github.com/TheSpeedX/commit-bot\n'
			print 'For Any Queries Join Me On WhatsApp!!!'
			print '\t    Group Link: http://bit.do/speedxgit'
			print '\n             Mail: ggspeedx29@gmail.com'
			print '\n  YouTube Channel: https://www.youtube.com/c/GyanaTech'
			raw_input('\n\nPress Enter To Continue...')
			continue
		print '[+] Initializing....'
		if os.path.exists('test')==False:
			os.system('mkdir test')
			print '[+] Test Directory Not Found Creating One ....'
		else:
			os.system('cd test && rm -rf *')
			print '[+] Test Directory Found Using It ....'
		os.system('rm -rf .git>temp.speedx.xxxxx')
		print '[+] Preparing Directory...'
#		os.system('cd test && git init')
		print '[+] Pulling REMOTE Repository To Local Directory ...'
#		os.system('cd test && git pull')
		os.system('cd test && git clone '+gu)
		rn=gu[gu.rfind('/')+1:]
		os.system('mv -f test/'+rn+'/*   test >>temp.speedx.xxxxx')
		os.system('mv -f test/'+rn+'/.??* test>>temp.speedx.xxxxx')
		os.system('cd test && git remote add origin '+gu)
		os.system('rm -f temp.speedx.xxxxx')
		os.system('cd test && rm -rf '+rn)
		print '[+] Repository Successfully Pulled '
		if not os.path.exists('test/README.md'):
			os.system('touch test/README.md')
		f=open('test/temp.speedx','w')
		f.write(chr(35)+' This Repo Was Commited By SpeedX\'s Commit Bot\n')
		f.write(chr(35)+chr(35)+chr(35)+' GITHUB LINK\n')
		f.write( '<a href=\'https://github.com/thespeedx/commit-bot\'> Click Here </a>\n\n')
		f.close()
#		os.system('cd test && echo '+chr(35)+' This Repo Was Commited By SpeedX\'s Commit Bot >temp.speedx')
#		os.system('cd test && echo '+chr(35)+chr(35)+chr(35)+' GITHUB LINK >>temp.speedx')
#		os.system('cd test && echo <a href=\'https://github.com/thespeedx/commit-bot\'> Click Here </a> >>temp.speedx')
		os.system('cat test/temp.speedx test/README.md test/temp.speedx > test/tmp.xxxx ')
		os.system('cd test && mv tmp.xxxx README.md')
		os.system('cd test && rm temp.speedx')
		os.system('cd test && git config user.name \"'+gn+'\"')
		os.system('cd test && git config user.email \"'+ge+'\"')
		os.system('cd test && git add .')
		print '[+] Directory Initialized '
		print '[+] Starting Commits To Gain Contribution...'
		for i in progressbar.progressbar(range(nc-1),redirect_stdout=True):
			os.system('echo THIS IS A COMMIT BY SPEEDX COMMIT BOT >> test/temp.speedx.xxx')
			os.system('cd test && git add temp.speedx.xxx . >/dev/null')
#			print '[-] Commit Number: '+str(i+1)
			os.system('cd test && git commit -m \'Commit By SpeedX Bot!!! \'>/dev/null')
		print '\n[+] Cleaning Repository...'
		os.system('rm test/temp.speedx.xxx')
		os.system('cd test && git gc')
		print '[+] Repository Cleaned '
		print '[-] Final Commit'
		os.system('cd test && git add .')
		os.system('cd test && git commit -m \'Commit By SpeedX Bot!!! \'')
		print '[+] Pushing Repo To Remote URL: '+gu
		os.system('cd test && git push -u --force origin master')
		print '[+] '+str(nc)+' Commits Done ... \n\t\tYou Can See it in your Contributions Soon\n\tIf You Don\'t Check Notes in README.md'
		print '[+] Closing Bot....'
		break
	elif not inp.find('2')==-1:
		os.system('clear')
		print '                       HELP'
		print '           -----------------------------'
		print logo+'\n'
		print 'This is A COMMIT BOT Created By SpeedX to get CONTRIBUTIONS For FREE...'
		print 'This Script Generates Fake Commits And is Very Fast....'
		print '\nALWAYS USE AN EMPTY REPOSITORY WITH AN INITIAL COMMIT FOR COMMIT BOT!!\n'
		print 'We Take The Following Inputs:\n'
		print '\t Number Of Commits -   To Generate That Amount Of Fake Commits '
		print '\t Repository URL    -   To Push And Pull Code To/From That Repository(Must Be Yours)'
		print '\t Github Username   -   Sometimes Github Asks For UserName (Enter A Real One) ...'
		print '\t Github Email      -   Sometimes Github Asks For Email (Enter A Real One) ...'
		print '\nWe Never Keep You Github Username, Email or Password... '
		print 'If You Don\'t Trust Us Then Push The Repository Yourself After Successful Commits By:'
		print '\t\tcd test && git push -u --force origin master'
		print '\n\tFor More Details Check README.md\nHope You Liked This Project!!!'
		print 'You can Check My Other Projects Here: https://github.com/TheSpeedX'
		print 'For Any Queries Join Me On WhatsApp!!!'
		print '\t    Group Link: http://bit.do/speedxgit'
	        print '\n             Mail: ggspeedx29@gmail.com'
		print '\n  YouTube Channel: https://www.youtube.com/c/GyanaTech'
		raw_input('\n\nPress Enter To Continue...')
	elif not inp.find('3')==-1:
		break
	else:
		print "Invalid Input !!!\nTry Again!!!\n Press Enter To Continue..."
		raw_input()

print logo
print '\nThanks For Using My Project'
print 'PLEASE LEAVE A STAR IT, FORK IT, WATCH IT IF YOU LIKE IT'
print 'You can Check My Other Projects Here: https://github.com/TheSpeedX'
print 'For Any Queries Join Me On WhatsApp!!!'
print '\t    Group Link: http://bit.do/thespeedx'
print '\n             Mail: ggspeedx29@gmail.com'
print '\n  YouTube Channel: https://www.youtube.com/c/GyanaTech'
sys.exit(0)
