# Lab Report 4 Week 5

Summary: For my lab report this week, I will be choosing the "grep" command as my research command. Below will be three alternative ways you can use "grep", and three examples each of using that alternative version.  
  
    
    
## grep -c 

    911report grep -c After chapter-10.txt
    4

This example is finding all the lines that have the matching parameter "After". This can be useful for finding specific words.


    biomed grep -c "last two decades" 1471-213X-1-11.txt
    1

This example is now having a longer phrase, if you want to see if your line repeats.


    plos grep -c a journal.pbio.0020019.txt
    140

This example is finding the word "a" which is a good way to see how many common words you are using.

## grep -n

    911report grep -n "Al Qaeda" chapter-5.txt
    185:                share. Al Qaeda associate Abu Zubaydah has expressed more qualified admiration for
    193:            Al Qaeda's success in fostering terrorism in Southeast Asia stems largely from its
    212:                KSM, Hambali soon began dealing with Atef as well. Al Qaeda began funding JI's
    215:                bomb-making materials and other supplies. Al Qaeda would underwrite operations,
    1076:            Al Qaeda appears to have relied on a core group of financial facilitators who raised
    1081:                their donations. Al Qaeda and its friends took advantage of Islam's strong calls for
    1086:            Al Qaeda also collected money from employees of corrupt charities.
    1115:            Al Qaeda also sought money from wealthy donors in other Gulf states.
    1116:            Al Qaeda frequently moved the money it raised by hawala, an informal and ancient
    1132:                annual operating budget. Al Qaeda funded salaries for jihadists, training camps,
    1140:            Al Qaeda has been alleged to have used a variety of illegitimate means, particularly
    1155:                significance. Al Qaeda had many avenues of funding. If a particular funding source

This can be used to find where exactly a word is you are looking for.  



    911report grep -n "HOW TO DO IT? A DIFFERENT WAY OF ORGANIZING THE GOVERNMENT" chapter-
    13.1.txt
    4:            HOW TO DO IT? A DIFFERENT WAY OF ORGANIZING THE GOVERNMENT

This can be used to find a line where you wrote a specific sentence.   



    About_LSC grep -n "Kennedy" commission_report.txt
    32:to the President John Kennedy, Director of A dministration and
    3194:S16911 (Oct. 17, 1986) (statement of Sen. Kennedy); March Comments

This can be used if you are looking how many times a specific name comes up in a document.

## grep -e

    911report grep -e ", but" chapter-5.txt
                    experiences there as a student, but rather from his violent disagreement with U.S.
                    attempted to follow through on the cargo carriers plan, but he was arrested in
                    KSM's ideas without much comment, but did ask KSM formally to join al Qaeda and move
                    Ladin reportedly liked this proposal, but he instructed KSM to concentrate on the
                    officials searched his carry-on bag and even opened the toiletries kit, but just
                    passengers as hostages, but only speculatively. Khallad admits being aware at the
                    earlier. Nibras and Quso were bringing Khallad money from Yemen, but were stopped in
                    same hotel, but Khallad insists that the two sets of operatives never met with each
                    operation, but added the enormous advantages of fluency in English and familiarity
                When Atta arrived in Germany, he appeared religious, but not fanatically so. This
                    Binalshibh in Yemen remembers him as "religious, but not too religious." From 1987
                    semester starting in August 1998, but back in Bonn. Shehhi initially flouted this
                In Hamburg, Jarrah had a succession of living accommodations, but he apparently never
                        described himself as a weak Muslim when he was home in Morocco, but much more
                    tradecraft was not especially sophisticated, but it was good enough. They moved,
                    significant sum, to be sure, but not a $300 million fortune that could be used to
                Saudi Arabia has long been considered the primary source of al Qaeda funding, but we
                    fund-raisers and operatives outside of Afghanistan, but there is little evidence

 You cannot see it in the code block, but it is highlighted in red everytime there is a ", but". This could be useful for how repetitive your text is.
    
    911report grep -e "remain independent" chapter-5.txt
            KSM declined. He preferred to remain independent and retain the option of working

This could be to make sure you don't have any patterns in your file.    

    Media grep -e "?" Abuse_penalties.txt
    orders? That it's OK to abuse women in Schuylkill County, because
    you'll only get a slap on the wrist?"

This can be used to see how many questions you have in your file.