For my Lab 5 report I am doing a remake of Lab report 3 with examples of Grep instead of Find.

I used ChatGpt -- with the prompt generate examples of using the Grep command


Example 1 ---> grep n gets the specfic line and line # in the txt file as shown by the 2 examples below 

Example 1.1
```
nilaybhoot@Nilays-MacBook-Pro berlitz1 % grep -n "Recommended Hotels" HandRHongKong.txt
6:        Recommended Hotels
```


Example 1.2
```
nilaybhoot@Nilays-MacBook-Pro berlitz1 % grep -n "The following hotels are listed alphabetically in three" HandRLosAngeles.txt
7:        The following hotels are listed alphabetically in three
```



Example 2 ---> grep -r gives every instantce of the string from all the files in the given directory as shown by the examples below

Example 2.1 

```
nilaybhoot@Nilays-MacBook-Pro OUP % grep -r "money" Abernathy 

Abernathy/ch3.txt:The growth in consumer expenditures did not rise commensurately with the boom in retail space. The apparel and upkeep share of household expenditures in the Consumer Price Index fell from 10.6 percent in 1963 to 5.5 percent in 1995. Per capita expenditure for apparel and related services declined from $1,710 in 1992 to $1,698 in 1994 (in current dollars).19 And these downward expenditure trends occurred in the face of growth in the average number of outerwear garments consumed per capita: from 14.3 garments in 1967 to 28.7 garments in 1995.20 In other words, the amount of money spent by an average consumer per garment fell over this period, reflecting in part more casual workplaces, which allow people to spend less on clothing for work, and intense price competition. Retailers with more and more floor space were chasing fewer and fewer apparel-consumption dollars.21
Abernathy/ch6.txt:After completing the process of developing a demand forecast for each SKU, a retailer must determine how much of each item to stock on the shelves of its stores. Retailers have an incentive to stock high levels of inventory: They want both to provide sufficient display stock to attract customers???empty shelves are not inviting???and to have products available for those who wish to purchase them. Yet carrying inventory is expensive: Retailers pay capital costs for having their money tied up in inventory, for the physical floor space necessary to store goods, and for handling, managing, and monitoring the inventory.10 Most important, they pay a ???risk premium??? for carrying products that might become obsolete, either because they are damaged or fall out of fashion.
Abernathy/ch8.txt:The percentage of the population wearing factory-made apparel has grown steadily since the nineteenth century. Some still rely on custom-made clothing, especially those who have to go this route because of their size and shape or those with the money to afford custom tailoring. Although many might like to have customized clothing, few consider it a realistic option. It is only recently that ???mass customization??? may make sense for both consumers and apparel-makers.10
Abernathy/ch8.txt:Our survey indicates that the average length of time it takes to get a garment ready for sewing, from issuing the order for a given marker to having the pieces cut and otherwise prepared, is 4.9 working days. The cut parts are then sent to sewing areas or other factories. If the sewing room is in the same building as the cutting room, then cut goods are sent over many times a day. If the sewing factory is far away, then a shipment once a week is typical. Reducing the time from placement of the order to cut goods in the sewing room requires decreasing both the time it takes to complete preassembly and the wait for delivery to the sewing room. Indeed, logistical considerations enter assembly well before garments are finally sewn together. Time really is money in today???s apparel industry, a theme we will expand on in the next two chapters.
Abernathy/ch14.txt:Based on our observations of apparel suppliers, coming up with the money for new technologies and practices seems to be less of an impediment than altering basic management conceptions about using these technologies for planning and production. Many of the business units in our sample have adopted specific practices without changing their approach to using them together to compete in an integrated channel. They continue to draw on traditional conceptions of planning, production, and sourcing???in other words, they still think in terms of large orders of their products, placed months before delivery is expected. Needless to say, these business units have not fully benefited from the investments they have made.
```

Example 2.2
```
nilaybhoot@Nilays-MacBook-Pro travel_guides % grep -r "Acre" berlitz1 

berlitz1/HistoryIsrael.txt:        won back Akko (Acre) but failed to regain Jerusalem. Other Crusades
berlitz1/WhereToEgypt.txt:        from a Crusader church in Acre (now Israel) when it was overrun by Arab
berlitz1/WhereToIsrael.txt:        Crusader town of Akko, better known as Acre.
berlitz1/WhereToIsrael.txt:        Akko (Acre)
berlitz1/WhereToIsrael.txt:        here in 1099, and Acre became the Crusaders??? capital and a key port in
berlitz1/HandRIsrael.txt:        Akko (Acre)
berlitz1/HandRIsrael.txt:        (04) 912 891, fax (04) 910 434. Acre???s finest lodgings, with a beach
berlitz1/HandRIsrael.txt:        Akko (Acre)
berlitz1/WhatToJamaica.txt:        you travel south, the landscape changes. Acres of grassland surround
```


Example 3 --> grep -c gets the amount of times the given string is repeated in the given txt file

Example 3.1
```
nilaybhoot@Nilays-MacBook-Pro berlitz1 % grep -c "hotel" HandRIsrael.txt


14
```

Example 3.2
```
nilaybhoot@Nilays-MacBook-Pro berlitz1 % grep -c "hotel" HandRJamaica.txt


6
```

Example 4.1 --> grep -v gets all sentences in the given files without the given phrase

```
nilaybhoot@Nilays-MacBook-Pro berlitz1 % grep -v "Hotel" HandRHawaii.txt


  
  
    
      
        Oahu (Including Honolulu)
        Aston Waikiki Sunset $$$ 229 Paoakalani Avenue, Honolulu, HI
        96815; Tel. (808) 922-2700 or (800) 336-5599; fax (808) 922-8785;
        <www.aston-hotels.com>. One of Aston???s many condominium resort
        properties, this modern high-rise has large rooms with complete
        kitchens. Lanais afford views of the Diamond Head end of Waikiki Beach.
        410 rooms.
        Halekulani $$$$ 2199 Kalia Road, Honolulu, HI 96815; Tel.
        (808) 923-2311 or (800) 367-2343; fax (808) 926-8004;
        <www.halekulani.com>. Very large rooms, most facing the ocean,
        and luxurious bathrooms with robes, make this a ???House Befitting
        Heaven,??? the meaning of its Hawaiian name. With plenty of beachfront, a
        top French restaurant (La Mer), and the serene House Without A Key
        outdoor lounge for sunset drinks, Halekulani is a complete resort. 454
        rooms.
        Hilton Hawaiian Village $$$???$$$$ 2005 Kalia Road, Honolulu,
        HI 96815; Tel. (808) 949-4321 or (800) 445-8667; fax (808) 947-7898;
        <www.hawaiianvillage.hilton.com>. Waikiki???s larg??est resort
        covers 22 beachfront acres of gardens, lagoons, waterfalls, coconut
        palms, and swimming pools. There are dozens of shops, a spa, and a
        branch of the Bishop Museum in the Kalia Tower. Families love this
        city-within-a-city on the beach. 2,998 rooms.
        Hyatt Regency Waikiki $$$???$$$$ 2424 Kalakaua Avenue,
        Honolulu, HI 96815; Tel. (808) 923-1234 or (800) 233-1234; fax (808)
        923-7839; <www.hyattwaikiki.com>. The Hyatt???s two
        recently-renovated 40-story towers cover a city block at the Diamond
        Head end of Waikiki???s shopping avenue (across the street from the
        beach). 1,241 rooms.
        Ihilani Resort & Spa $$$$ Ka Olina Resort & Marina,
        92-1001Olani Street. Kapolei, HI 96707; Tel. (808) 679-0079 or (800)
        626-4446; fax (808) 679-0080; <www.ihilani.com>. A luxury resort
        on the west side of Oahu, expertly managed by JW Marriott, Ihilani is
        situated within a 640-acre resort community that provides golf, tennis,
        3 miles of beaches and lagoons, and a world-class spa within a
        half-hour drive of Honolulu. 387 rooms.
        Kahala Mandarin Oriental Hawaii $$$$ 5000 Kahala Avenue,
        Honolulu, HI 96816; Tel. (808) 739-8888 or (800) 367-2525; fax (808)
        739-8800; <www.mandarin-oriental.com/??kahala>. Graceful, elegant,
        and refurbished for the new century, the venerable Kahala artfully
        mixes Hawaiian, Asian, and international touches. There???s a private
        beach, swimming pool, and lagoon with resident turtles and dolphins.
        402 rooms.
        Outrigger Reef $$$ 2169 Kalia Road, Honolulu, HI 96815; Tel.
        (808) 923-3111 or (800) 462-6262; fax (808) 924-4957;
        <www.outrigger.com>. This 17-story tower, perched on one of the
        best stretches of Waikiki oceanfront, is more deluxe than most
        Outrigger and related Ohana hotels. Its rooms, views, and amenities
        rival those of more expensive hotels on the same beach. 883 rooms.
        96815; Tel. (808) 922-1233 or (800) 367-6060; fax (808) 922-0129;
        <www.pacificbeachhotel.com>. The hotel???s twin towers, located at
        the Diamond Head end of Waikiki, are a block from Kuhio Beach. Rooms
        have private lanais, refrigerators, and coffeemakers. 830 rooms.
        Royal Hawaiian $$$$ 2259 Kalakaua Avenue, Honolulu, HI
        96815; Tel. (808) 923-7311 or (800) 325-3535; fax (808) 924-7098;
        <www.royal-hawaiian.com>. Waikiki???s ???Pink Palace,??? built by the
        Matson steamship line, has been a landmark since it opened in 1927 on
        the site of a royal summer palace on the beach. 527 rooms.
        Sheraton Moana Surfrider $$$$ 2365 Kalakaua Avenue,
        Honolulu, HI 96815; Tel. (808) 922-3111 or (800) 325-3535; fax (808)
        923-0308; <www.sheraton-moana.com>. The colonial porte coch??re
        sets the tone for Waikiki???s most charming historic hotel, which opened
        in 1901. The hotel???s original banyan wing has been restored to its old
        elegance. The amenities and daily activities (including hotel tours)
        are top-notch, and the buffet meals, especially on Sunday, on the
        beachfront veranda near the courtyard banyan tree couldn???t be more
        romantic. 793 rooms.
        Sheraton Princess Kaiulani $$$???$$$$ 120 Kaiulani Avenue,
        Honolulu, HI 96815; Tel. (808) 922-5811 or (800) 325-3535; fax (808)
        931-4526; <www.princess-kaiulani.com>. A block removed from
        Waikiki Beach, but a few steps from the heart of the Waikiki shopping
        district, the Princess Kaiulani dates back to 1955, but the rooms are
        all updated and its 29-story tower is much newer. 1,150 rooms.
        Sheraton Waikiki $$$???$$$$ 2255 Kalakaua Avenue, Honolulu,
        HI 96815; Tel. (808) 922-4422 or (800) 325-3535; fax (808) 923-8785;
        <www.sheraton-waikiki.com>. With two 30-story towers, this is
        largest of Sheraton???s four Waikiki beachfront hotels, with the most
        services and room options. 1,852 rooms.
        Maui
        Alanui, Wailea,, HI 96753; Tel. (808) 875-1234 or (800) 888-6100; fax
        (808) 874-2411; <www.grandwailea.com>. Maui???s ultimate fantasy
        resort?????????said to be the most expensive resort ever built?????????is a
        favorite with families. 780 rooms.
        96713; Tel. (808) 248-8211 or (800) 321-4262; fax (808) 248-7202;
        <www.hotelhanamaui.com>. At the end of the legendary road to Hana
        on Maui???s remote and lush east shore, this quiet upscale resort on 66
        acres with a wild volcanic oceanfront is the oldest in Maui (1946). The
        cottages near the shoreline, styled like plantation homes with large
        covered porches, are luxurious within; some come with private hot tubs.
        66 rooms.
        Hyatt Regency Maui $$$$ 200 Nohea Kai Drive, Lahaina,, HI
        96761; Tel. (808) 661-1234 or (800) 233-1234; fax (808) 667-4714;
        <www.maui.hyatt.com>. At the south end of the Kaanapali Beach
        resort complex, the Hyatt Regency is a 40-acre tropical fantasy resort,
        with exotic birds, waterfalls, garden atriums, and sculpted swimming
        pools. 806 rooms.
        Road, Napili Beach, Lahaina, HI 96761; Tel. (808) 669-6205 or (800)
        367-5034; fax (808) 669-0129; <www.mauian.com>. Well north of
        Kaanapali Beach, the Mauian is a Hawaiian-owned hotel dating back to
        1959, restored to its original ambience. All units are equipped with
        kitchens and ceiling fans (no air-conditioning, TVs, or phones). The
        free breakfast is a delight. 44 rooms.
        Ohana Maui Islander $$ 660 Wainee Street, Lahaina, HI
        96761; Tel. (808) 667-9766 or (800) 462-6262; fax (808) 661-3733;
        <www.ohanahotels.com>. This is Ohana???s first hotel on Maui,
        equipped with a pool and tennis courts. 360 rooms.
        Outrigger Wailea Resort $$$???$$$$ 3700 Wailea Alanui,
        Wailea, HI 96753; Tel. (808) 879-1922 or (800) OUT-RIGGER; fax (800)
        622-4852; <www.outrigger.com>. This 22-acre oceanfront resort,
        adjacent to two of the best beaches on the Kona Coast, has a
        spectacular open lobby and fine rooms with private balconies. 516
        rooms.
        Ritz-Carlton, Kapalua $$$$ One Ritz-Carlton Drive,
        Kapalua,, HI 96761; Tel. (808) 669-6200 or (800) 262-8440; fax (808)
        665-0026; <www.ritzcarlton.com>. The most northerly of the
        western Maui oceanfront resorts, the Ritz-Carlton is a grand hotel with
        hints of tropical plantation days, set amidst rugged coves and
        mountains.548 rooms.
        Alanui, Kihei, HI 96753; Tel. (808) 874-1111 or (800) 321-6284; fax
        (808) 879-8763; <www.westin.com>. The most southwesterly of
        Maui???s big resorts, the Prince has a pretty beach facing Molokini Isle.
        The rooms are large, lavish, and uncluttered, all with private
        ocean-view lanais. The courtyard grounds are lush with gardens and
        immense koi pools. 310 rooms.
        Big Island of Hawaii
        Ohana Keauhou Beach Resort $$???$$$ 78-6740 Alii Drive,
        Kailua-Kona, HI 96740; Tel. (808) 322-3441 or (800) 462-6262; fax (808)
        322-3117; <www.ohanahotels.com>. This old-fashioned resort from
        the 1970s has been fully renovated; rooms are spar??kling and modern.
        The grounds, including a royal sacred pool, are lush, and a few steps
        away is one of the island???s best snorkeling and swimming beaches. 311
        rooms.
        Chalet Kilauea $$???$$$ P.O. Box 998, Volcano, HI 96785; Tel.
        (808) 967-7786 or (800) 937-7786; fax (800) 577-1849 or (808) 967-8660;
        <www.volcano-hawaii.com>. Brian and Lisha Crawford are the kings
        of bed & breakfast accommodations in the Volcano area. They have
        rooms and houses to fit many tastes and budgets, from the lavish to the
        thrifty. The Chalet Kilauea, the hub of this little empire, serves
        gourmet breakfasts and afternoon teas. 6 rooms.
        Four Seasons Resort Hualalai $$$$ P.O. Box 1269,
        Kailua-Kona, HI 96745; Tel. (808) 325-8000 or (888) 336-5662; fax (808)
        325-8100; <www.fourseasons.com>. Upscale bungalows with slate
        floors, private gardens, and spacious lanais create a relaxing hideaway
        on the beach. There???s a private championship golf course, tennis court
        complex, and five swimming pools facing the ocean. 243 rooms.
        Hilton Waikoloa Village $$$$ 69-425 Waikoloa Beach Drive,
        Waikoloa, HI 96738; Tel. (808) 886-1234 or (800) HILTONS; fax
        (808)886-2900; <www. hiltonwaikoloavillage.com>. A fantasy resort
        for the whole family, with trams and launches to take guests to their
        rooms, the Hilton is best known for its swim-with-the-dolphins program.
        There???s also a 1-acre swimming pool with water slides and a vast array
        of amenities and services all over the 62-acre (25-hectare) oceanfront
        grounds. 1,240 rooms.
        Coast, HI 96743; Tel. (808) 882-7222 or (800) 735-1111; fax (808)
        880-3112; <www.maunakeabeachhotel.com>. Built in 1965 by Laurance
        Rockefeller, this was the first great resort to be carved out of the
        lava on the Kohala Coast. It was lauded as the best island resort in
        the world for years, and it is still one of Hawaii???s premier oceanfront
        resorts, with a vast art collection, a great beach, a major golf
        course, a loyal staff, and a style all its own. 310 rooms.
        Drive, Kohala Coast, HI 96743; Tel. (808) 885-6622 or (800) 367-2323;
        fax (808) 885-4556; <www.maunalani.com>. Spacious rooms with
        lanais face the beach and an atrium complex of gardens and pools in
        this posh resort, the Mauna Kea???s main rival. The shoreline trail leads
        through ancient fishponds and lagoons where endangered baby sea turtles
        are raised and released every July 4th. At the end of the trail is a
        cove and reef where the freed turtles await swimmers and snorkelers.
        350 rooms.
        Outrigger Waikoloa Beach $$$ 69-275 Waikoloa Beach Drive,
        Kamuela,, HI 96738; Tel. (808) 886-6789 or (800) 922-5533; fax (808)
        886-7852; <www.outrigger.com>. Renovated in 2000, this
        full-service resort fronts a tremendous swimming and snorkeling beach
        with dozens of turtles. 545 rooms.
        Kauai
        Hanalei Colony Resort $$???$$$ 5-7130 Kuhio Highway, Hanalei,
        HI 96714; Tel. (808) 826-6235 or (800) 628-3004; fax (808) 826-9893;
        <www.marriott.com>. Nearly at the end of a winding road to the Na
        Pali Coast, these condominium units are beginning to show their age,
        but they come with complete kitchens, a white-sand beach with tide
        pools, and looming mountain peaks out of Bali Hai. No TVs or phones
        ring out in this paradise. 48 rooms.
        Kauai Marriott Resort & Beach Club $$$$ Kalapaki Beach,
        Lihue, HI 96766; Tel. (808) 245-5050 or (800) 228-9290; fax (808)
        245-5049; <www.hcr.com>. Hit hard by Hurricaine Iniki, this
        lavish resort finally reopened, retaining its informal feel, its fine
        golf courses, its lagoons with exotic animals on the isles, and some of
        the best hotel pools and swimming beaches in Hawaii. 419 rooms.
        Poipu Kapili $$$ 2221 Kapili Road, Koloa, HI 96756; Tel.
        (808) 742-6449 or (800) 443-7714; fax (808) 742-9162;
        <www.poipukapili.com>. These upscale oceanfront condominiums are
        among the best-maintained on the southern shore. Units are very large,
        fully equipped (some with washers and dryers). Mag??nif??i??cent sunsets.
        60 rooms.
        Sheraton Kauai Resort $$$$ 2440 Hoonani Road, Koloa, HI
        96756; Tel. (808) 742-1661 or (888) 847-0208; fax (808) 923-2023;
        <www.sheraton-kauai.com>. An all-inclusive resort on the Poipu
        shore, Sheraton offers large rooms in three buildings, including two
        buildings facing a lava rock shoreline. Swimming pools, spa, tennis,
        and children???s programs attract couples and families. 413 rooms.
        Molokai
        Ke Nani Kai Resort $$ Kaluakoi Resort, Kaluakoi Road,
        Maunaloa, HI 96770; Tel. (808) 552-2761 or (800) 888-2791; fax (808)
        552-0045; <www.marcresorts.com>. A family resort on the west side
        of the island, Ke Nani Kai consists of spacious fully-appointed
        apartments, a swimming poo1, tennis courts, and a golf course. Walk to
        Kepuhi Beach, drive to 3-mile-long Papohaku Beach. 120 rooms.
        Molokai Ranch & Lodge $$$???$$$$ P.O. Box 259, Maunaloa,
        HI 96770; Tel. (808) 552-2741 or (877) 726-4656; fax (808) 534-1606;
        <www.molokai-ranch.com>. Still a 54,000-acre working cattle and
        horse ranch on the west side of the island, this is Molokai???s most
        deluxe resort, with fine rooms with large lanais in the new lodge and
        three clusters of upscale ???tentalows??? and yurts, including one deluxe
        camp right on the beach. Outdoor activities run the gamut: horseback
        riding, ocean kayaking, excellent mountain biking, clay shooting,
        hiking. 60 tentalows, 20 yurts, 22 lodge rooms.
        Lanai
        Tel. (808) 565-7211 or (800) 795-7211; fax (808) 565-6450;
        <www.onlanai.com>. A 1923 pineapple plantation guesthouse for
        company executives, this country inn near the town square caters to
        outdoor enthusiasts. Rooms are quaint, with no air-conditioning.
        Breakfast included. 11 rooms.
        Lodge at Koele $$$$ P.O. Box 310, Lanai City, HI 96793;
        Tel. (808) 565-7300 or (800) 321-4666; fax (808) 565-4561;
        <www.lanai-resorts.com>. Lanai???s upcountry, very upscale resort
        is appointed like an Old English estate, with writing desks,
        four-poster beds, library, music room. The 21-acre grounds include a
        croquet court, lawn bowling, horseback-riding stables, formal gardens,
        and a world-class golf course. 102 rooms.
        Tel. (808) 565-7700 or (800) 321-4666; fax (808) 565-2483;
        <www.lanai-resorts.com>. A full-service, quite plush resort on
        sports, golf, tennis, a spa, and jeep tours. 250 rooms.
      
```


Example 4.2
```
nilaybhoot@Nilays-MacBook-Pro berlitz1 % grep -v "the" HandRIbiza.txt 


  
  
    
      
        Recommended Hotels
        The establishments listed below offer a cross-section of
        island comes with chips (french fries).
        offfical government rating system.
        expect to pay for a three-course meal for two, excluding wine, tax and
        ???less than 5,000 ptas.
        ??????5,000???8,000 ptas.
        ?????????more than 8,000 ptas.
```




