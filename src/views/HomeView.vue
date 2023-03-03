<template>
  <div class="max-w-[1400px] mx-auto">
    <div class="min-w-[800px] w-full px-8 mt-8">
      <div class="inline-block text-white font-semibold text-xl">
        Hello, we are QKIT Company
      </div>

      <div class="py-2"></div>

      <div class="flex w-full justify-between gap-8">
        <div class="xl:w-1/3 lg:w-1/2 md:w-full">
          <MixesInspiredBy
            class="pb-1.5"
            to="/artist"
            by="Imagine Dragons"
            text="Believer - Imagine Dragons (Lyrics)"
            image="https://img.youtube.com/vi/SxEbPvXaQlA/maxresdefault.jpg"
          />
          <MixesInspiredBy
            class="pb-1.5"
            to="/artist"
            by="James Arthur"
            text="Ed Sheeran - Shape of You (Lyrics)"
            image="https://img.youtube.com/vi/rverDjn4MXY/maxresdefault.jpg"
          />
          <MixesInspiredBy
            class="pb-1.5"
            to="/artist"
            by="Ed Sheeran"
            text="James Arthur ft. Anne-Marie (Lyrics)"
            image="https://img.youtube.com/vi/ddO3wIsDrRQ/maxresdefault.jpg"
          />
        </div>
        <div class="xl:w-1/3 w-1/2">
          <MixesInspiredBy
            class="pb-1.5"
            to="/artist"
            by="James Arthur"
            text="Ed Sheeran - Shape of You (Lyrics)"
            image="https://img.youtube.com/vi/rverDjn4MXY/maxresdefault.jpg"
          />
          <MixesInspiredBy
            class="pb-1.5"
            to="/artist"
            by="Imagine Dragons"
            text="Believer - Imagine Dragons (Lyrics)"
            image="https://img.youtube.com/vi/SxEbPvXaQlA/maxresdefault.jpg"
          />
          <MixesInspiredBy
            class="pb-1.5"
            to="/artist"
            by="Ed Sheeran"
            text="James Arthur ft. Anne-Marie (Lyrics)"
            image="https://img.youtube.com/vi/ddO3wIsDrRQ/maxresdefault.jpg"
          />
        </div>
        <div class="xl:w-1/3 lg:w-1/2 md:w-full">
          <MixesInspiredBy
            class="pb-1.5"
            to="/artist"
            by="Ed Sheeran"
            text="James Arthur ft. Anne-Marie (Lyrics)"
            image="https://img.youtube.com/vi/ddO3wIsDrRQ/maxresdefault.jpg"
          />
          <MixesInspiredBy
            class="pb-1.5"
            to="/artist"
            by="Imagine Dragons"
            text="Believer - Imagine Dragons (Lyrics)"
            image="https://img.youtube.com/vi/SxEbPvXaQlA/maxresdefault.jpg"
          />
          <MixesInspiredBy
            class="pb-1.5"
            to="/artist"
            by="James Arthur"
            text="Ed Sheeran - Shape of You (Lyrics)"
            image="https://img.youtube.com/vi/rverDjn4MXY/maxresdefault.jpg"
          />
        </div>
      </div>
    </div>

    <div class="px-8 mt-8 min-w-[800px]">
      <div class="text-white text-xl font-semibold inline-block">
        Made for you
      </div>

      <div class="py-2"></div>

      <div class="flex justify-start gap-7">
        <MultiArtistSelect
          class="w-1/4"
          to="/artist"
          text="Bleeding Love, Bleeding Love, Dive, Be Alright"
          category="Ed Sheeran"
          :imgs="{
            one: 'https://www.liveabout.com/thmb/DNPhPFtAm2PDIFbcexbdNY2XG-g=/1500x0/filters:no_upscale():max_bytes(150000):strip_icc()/pop-music-57bce3863df78c87634ea806.jpg',
            two: 'https://blog.hootsuite.com/wp-content/uploads/2017/05/creative-commons-music-resources.png',
            three:
              'https://images.saymedia-content.com/.image/t_share/MTg3MTY3ODgyMjY4OTExNTAy/why-so-many-artists-hate-spotify.png',
            four: 'https://www.liveabout.com/thmb/DNPhPFtAm2PDIFbcexbdNY2XG-g=/1500x0/filters:no_upscale():max_bytes(150000):strip_icc()/pop-music-57bce3863df78c87634ea806.jpg',
          }"
        />
        <MultiArtistSelect
          class="w-1/4"
          to="/artist"
          text="Bleeding Love, Bleeding Love, Dive, Be Alright"
          category="Ed Sheeran"
          :imgs="{
            one: 'https://www.liveabout.com/thmb/DNPhPFtAm2PDIFbcexbdNY2XG-g=/1500x0/filters:no_upscale():max_bytes(150000):strip_icc()/pop-music-57bce3863df78c87634ea806.jpg',
            two: 'https://blog.hootsuite.com/wp-content/uploads/2017/05/creative-commons-music-resources.png',
            three:
              'https://images.saymedia-content.com/.image/t_share/MTg3MTY3ODgyMjY4OTExNTAy/why-so-many-artists-hate-spotify.png',
            four: 'https://www.liveabout.com/thmb/DNPhPFtAm2PDIFbcexbdNY2XG-g=/1500x0/filters:no_upscale():max_bytes(150000):strip_icc()/pop-music-57bce3863df78c87634ea806.jpg',
          }"
        />
        <MultiArtistSelect
          class="w-1/4"
          to="/artist"
          text="Bleeding Love, Bleeding Love, Dive, Be Alright"
          category="Ed Sheeran"
          :imgs="{
            one: 'https://www.liveabout.com/thmb/DNPhPFtAm2PDIFbcexbdNY2XG-g=/1500x0/filters:no_upscale():max_bytes(150000):strip_icc()/pop-music-57bce3863df78c87634ea806.jpg',
            two: 'https://blog.hootsuite.com/wp-content/uploads/2017/05/creative-commons-music-resources.png',
            three:
              'https://images.saymedia-content.com/.image/t_share/MTg3MTY3ODgyMjY4OTExNTAy/why-so-many-artists-hate-spotify.png',
            four: 'https://www.liveabout.com/thmb/DNPhPFtAm2PDIFbcexbdNY2XG-g=/1500x0/filters:no_upscale():max_bytes(150000):strip_icc()/pop-music-57bce3863df78c87634ea806.jpg',
          }"
        />
        <MultiArtistSelect
          class="w-1/4"
          to="/artist"
          text="Bleeding Love, Bleeding Love, Dive, Be Alright"
          category="Ed Sheeran"
          :imgs="{
            one: 'https://www.liveabout.com/thmb/DNPhPFtAm2PDIFbcexbdNY2XG-g=/1500x0/filters:no_upscale():max_bytes(150000):strip_icc()/pop-music-57bce3863df78c87634ea806.jpg',
            two: 'https://blog.hootsuite.com/wp-content/uploads/2017/05/creative-commons-music-resources.png',
            three:
              'https://images.saymedia-content.com/.image/t_share/MTg3MTY3ODgyMjY4OTExNTAy/why-so-many-artists-hate-spotify.png',
            four: 'https://www.liveabout.com/thmb/DNPhPFtAm2PDIFbcexbdNY2XG-g=/1500x0/filters:no_upscale():max_bytes(150000):strip_icc()/pop-music-57bce3863df78c87634ea806.jpg',
          }"
        />
      </div>
    </div>

    <div class="min-w-[800px] px-8 mt-8">
      <div class="py-2"></div>

      <p class="pb-6 text-center text-[#D1D1D6] text-sm">
        Follow artists you like by tapping the follow button.
      </p>

      <div class="flex justify-center gap-7 full">
        <div class="flex justify-center items-center relative">
          <img
            width="100"
            class="-left-40 rounded-full z-0 cursor-pointer absolute"
            src="https://upload.wikimedia.org/wikipedia/vi/f/f2/Taylor_Swift_-_Reputation.png"
          />
          <img
            width="115"
            class="-left-[80px] rounded-full z-10 cursor-pointer absolute"
            src="https://hips.hearstapps.com/hmg-prod/images/canadian-pop-musician-shawn-mendes-photographed-backstage-before-a-live-performance-at-the-hammersmith-apollo-in-london-on-may-5-2016-photo-by-will-ireland_total-guitar-magazine-via-getty-images-500.jpg"
          />
          <img
            width="160"
            class="rounded-full z-20 cursor-pointer"
            src="https://doanhnhanonline.com.vn/wp-content/uploads/2021/11/Thien-tai-am-nhac-DJ-Alan-walker-la-ai.jpeg"
          />
          <img
            width="115"
            class="-right-[80px] rounded-full z-10 cursor-pointer absolute"
            src="https://cdn.shopify.com/s/files/1/0130/8714/6043/products/1_f2fad97f-dd0d-4191-89ff-8ab7c4c2c3b7.jpg?v=1649067718"
          />
          <img
            width="100"
            class="-right-40 rounded-full z-0 cursor-pointer absolute"
            src="https://yt3.googleusercontent.com/ytc/AL5GRJVjlPCxmYF_57UxAtrXUG69TQiWfEYy2KbWfhqe3VU=s176-c-k-c0x00fff-no-rj"
          />
        </div>
      </div>
      <div class="w-full flex justify-center p-3">
        <button
          type="button"
          class="text-white text-[15px] font-semibold rounded-full bg-[#bf325a] hover:bg-[#e87583] px-8 py-2 text-center"
        >
          ADD ARTISTS
        </button>
      </div>
    </div>

    <div class="mt-8 min-w-[800px]">
      <CustomCarousel
        category="New releases for you"
        :data="[
          {
            url: 'https://img.freepik.com/free-vector/electro-music-album_53876-67225.jpg?w=2000',
            song: 'Electronic',
            by: 'Electronic Music',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://d1csarkz8obe9u.cloudfront.net/posterpreviews/pink-cloud-cd-cover-music-design-template-258c703e9959b4635649e3944488c688_screen.jpg?ts=1631060402',
            song: 'CLOUD',
            by: 'Brian Sarubbi',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://pub-static.fotor.com/assets/projects/pages/55126b29-ff8d-475c-a5b5-d711e81caa6d/600w/purple-love-song-music-album-cover-64e5ec1b-0ed6-43a0-96e6-57a26534a584.jpg',
            song: 'Somebody that I like',
            by: 'Kate East',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://d1csarkz8obe9u.cloudfront.net/posterpreviews/creative-music-album-cover-design-template-f4ce22c75f3fff9758bc01250abc6e05_screen.jpg?ts=1594215605',
            song: 'Memories',
            by: 'Anthony Knight',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://img.freepik.com/free-vector/electro-music-album_53876-67225.jpg?w=2000',
            song: 'Electronic',
            by: 'Electronic Music',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://d1csarkz8obe9u.cloudfront.net/posterpreviews/pink-cloud-cd-cover-music-design-template-258c703e9959b4635649e3944488c688_screen.jpg?ts=1631060402',
            song: 'CLOUD',
            by: 'Brian Sarubbi',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://pub-static.fotor.com/assets/projects/pages/55126b29-ff8d-475c-a5b5-d711e81caa6d/600w/purple-love-song-music-album-cover-64e5ec1b-0ed6-43a0-96e6-57a26534a584.jpg',
            song: 'Somebody that I like',
            by: 'Kate East',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://d1csarkz8obe9u.cloudfront.net/posterpreviews/creative-music-album-cover-design-template-f4ce22c75f3fff9758bc01250abc6e05_screen.jpg?ts=1594215605',
            song: 'Memories',
            by: 'Anthony Knight',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://img.freepik.com/free-vector/electro-music-album_53876-67225.jpg?w=2000',
            song: 'Electronic',
            by: 'Electronic Music',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://d1csarkz8obe9u.cloudfront.net/posterpreviews/pink-cloud-cd-cover-music-design-template-258c703e9959b4635649e3944488c688_screen.jpg?ts=1631060402',
            song: 'CLOUD',
            by: 'Brian Sarubbi',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://pub-static.fotor.com/assets/projects/pages/55126b29-ff8d-475c-a5b5-d711e81caa6d/600w/purple-love-song-music-album-cover-64e5ec1b-0ed6-43a0-96e6-57a26534a584.jpg',
            song: 'Somebody that I like',
            by: 'Kate East',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://d1csarkz8obe9u.cloudfront.net/posterpreviews/creative-music-album-cover-design-template-f4ce22c75f3fff9758bc01250abc6e05_screen.jpg?ts=1594215605',
            song: 'Memories',
            by: 'Anthony Knight',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://img.freepik.com/free-vector/electro-music-album_53876-67225.jpg?w=2000',
            song: 'Electronic',
            by: 'Electronic Music',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://d1csarkz8obe9u.cloudfront.net/posterpreviews/pink-cloud-cd-cover-music-design-template-258c703e9959b4635649e3944488c688_screen.jpg?ts=1631060402',
            song: 'CLOUD',
            by: 'Brian Sarubbi',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://pub-static.fotor.com/assets/projects/pages/55126b29-ff8d-475c-a5b5-d711e81caa6d/600w/purple-love-song-music-album-cover-64e5ec1b-0ed6-43a0-96e6-57a26534a584.jpg',
            song: 'Somebody that I like',
            by: 'Kate East',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://d1csarkz8obe9u.cloudfront.net/posterpreviews/creative-music-album-cover-design-template-f4ce22c75f3fff9758bc01250abc6e05_screen.jpg?ts=1594215605',
            song: 'Memories',
            by: 'Anthony Knight',
            releasedOn: '03/03/2023',
          },
        ]"
      />
    </div>

    <div class="min-w-[800px] px-8 mt-8">
      <div class="text-white text-xl font-semibold inline-block">
        Highlights
      </div>

      <div class="py-3"></div>

      <div class="items-center flex gap-8">
        <div class="w-1/2 rounded-lg">
          <Highlights
            by="Some Artist #1"
            song="Awesome Song for you!"
            image="https://www.thechristianbeat.org/wp-content/uploads/2018/05/worthyofitall-1024x396.jpg"
          />
        </div>
        <div class="w-1/2 rounded-lg">
          <Highlights
            by="Some Artist #2"
            song="Awesome Song for you!"
            image="https://newmusicusa.org/wp-content/uploads/2016/01/turntablebanner-1024x394.jpg"
          />
        </div>
      </div>
    </div>

    <div class="mt-8 min-w-[800px]">
      <CustomCarousel
        category="Popular playlist"
        :data="[
          {
            url: 'https://img.freepik.com/free-vector/electro-music-album_53876-67225.jpg?w=2000',
            song: 'Electronic',
            by: 'Electronic Music',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://d1csarkz8obe9u.cloudfront.net/posterpreviews/pink-cloud-cd-cover-music-design-template-258c703e9959b4635649e3944488c688_screen.jpg?ts=1631060402',
            song: 'CLOUD',
            by: 'Brian Sarubbi',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://pub-static.fotor.com/assets/projects/pages/55126b29-ff8d-475c-a5b5-d711e81caa6d/600w/purple-love-song-music-album-cover-64e5ec1b-0ed6-43a0-96e6-57a26534a584.jpg',
            song: 'Somebody that I like',
            by: 'Kate East',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://d1csarkz8obe9u.cloudfront.net/posterpreviews/creative-music-album-cover-design-template-f4ce22c75f3fff9758bc01250abc6e05_screen.jpg?ts=1594215605',
            song: 'Memories',
            by: 'Anthony Knight',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://img.freepik.com/free-vector/electro-music-album_53876-67225.jpg?w=2000',
            song: 'Electronic',
            by: 'Electronic Music',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://d1csarkz8obe9u.cloudfront.net/posterpreviews/pink-cloud-cd-cover-music-design-template-258c703e9959b4635649e3944488c688_screen.jpg?ts=1631060402',
            song: 'CLOUD',
            by: 'Brian Sarubbi',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://pub-static.fotor.com/assets/projects/pages/55126b29-ff8d-475c-a5b5-d711e81caa6d/600w/purple-love-song-music-album-cover-64e5ec1b-0ed6-43a0-96e6-57a26534a584.jpg',
            song: 'Somebody that I like',
            by: 'Kate East',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://d1csarkz8obe9u.cloudfront.net/posterpreviews/creative-music-album-cover-design-template-f4ce22c75f3fff9758bc01250abc6e05_screen.jpg?ts=1594215605',
            song: 'Memories',
            by: 'Anthony Knight',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://img.freepik.com/free-vector/electro-music-album_53876-67225.jpg?w=2000',
            song: 'Electronic',
            by: 'Electronic Music',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://d1csarkz8obe9u.cloudfront.net/posterpreviews/pink-cloud-cd-cover-music-design-template-258c703e9959b4635649e3944488c688_screen.jpg?ts=1631060402',
            song: 'CLOUD',
            by: 'Brian Sarubbi',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://pub-static.fotor.com/assets/projects/pages/55126b29-ff8d-475c-a5b5-d711e81caa6d/600w/purple-love-song-music-album-cover-64e5ec1b-0ed6-43a0-96e6-57a26534a584.jpg',
            song: 'Somebody that I like',
            by: 'Kate East',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://d1csarkz8obe9u.cloudfront.net/posterpreviews/creative-music-album-cover-design-template-f4ce22c75f3fff9758bc01250abc6e05_screen.jpg?ts=1594215605',
            song: 'Memories',
            by: 'Anthony Knight',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://img.freepik.com/free-vector/electro-music-album_53876-67225.jpg?w=2000',
            song: 'Electronic',
            by: 'Electronic Music',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://d1csarkz8obe9u.cloudfront.net/posterpreviews/pink-cloud-cd-cover-music-design-template-258c703e9959b4635649e3944488c688_screen.jpg?ts=1631060402',
            song: 'CLOUD',
            by: 'Brian Sarubbi',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://pub-static.fotor.com/assets/projects/pages/55126b29-ff8d-475c-a5b5-d711e81caa6d/600w/purple-love-song-music-album-cover-64e5ec1b-0ed6-43a0-96e6-57a26534a584.jpg',
            song: 'Somebody that I like',
            by: 'Kate East',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://d1csarkz8obe9u.cloudfront.net/posterpreviews/creative-music-album-cover-design-template-f4ce22c75f3fff9758bc01250abc6e05_screen.jpg?ts=1594215605',
            song: 'Memories',
            by: 'Anthony Knight',
            releasedOn: '03/03/2023',
          },
        ]"
      />
    </div>

    <div class="px-8 mt-8 min-w-[800px]">
      <div class="text-white font-semibold text-xl inline-block">
        Highlights
      </div>

      <div class="py-3"></div>

      <div class="flex items-center gap-8">
        <div class="rounded-lg w-1/2">
          <Highlights
            by="Some Artist #1"
            song="Awesome Song for you!"
            image="https://newmusicusa.org/wp-content/uploads/2016/01/turntablebanner-1024x394.jpg"
          />
        </div>
        <div class="rounded-lg w-1/2">
          <Highlights
            by="Some Artist #2"
            song="Awesome Song for you!"
            image="https://www.thechristianbeat.org/wp-content/uploads/2018/05/worthyofitall-1024x396.jpg"
          />
        </div>
      </div>
    </div>

    <div class="mt-8 min-w-[800px]">
      <CustomCarousel
        category="New releases for you"
        :data="[
          {
            url: 'https://img.freepik.com/free-vector/electro-music-album_53876-67225.jpg?w=2000',
            song: 'Electronic',
            by: 'Electronic Music',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://d1csarkz8obe9u.cloudfront.net/posterpreviews/pink-cloud-cd-cover-music-design-template-258c703e9959b4635649e3944488c688_screen.jpg?ts=1631060402',
            song: 'CLOUD',
            by: 'Brian Sarubbi',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://pub-static.fotor.com/assets/projects/pages/55126b29-ff8d-475c-a5b5-d711e81caa6d/600w/purple-love-song-music-album-cover-64e5ec1b-0ed6-43a0-96e6-57a26534a584.jpg',
            song: 'Somebody that I like',
            by: 'Kate East',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://d1csarkz8obe9u.cloudfront.net/posterpreviews/creative-music-album-cover-design-template-f4ce22c75f3fff9758bc01250abc6e05_screen.jpg?ts=1594215605',
            song: 'Memories',
            by: 'Anthony Knight',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://img.freepik.com/free-vector/electro-music-album_53876-67225.jpg?w=2000',
            song: 'Electronic',
            by: 'Electronic Music',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://d1csarkz8obe9u.cloudfront.net/posterpreviews/pink-cloud-cd-cover-music-design-template-258c703e9959b4635649e3944488c688_screen.jpg?ts=1631060402',
            song: 'CLOUD',
            by: 'Brian Sarubbi',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://pub-static.fotor.com/assets/projects/pages/55126b29-ff8d-475c-a5b5-d711e81caa6d/600w/purple-love-song-music-album-cover-64e5ec1b-0ed6-43a0-96e6-57a26534a584.jpg',
            song: 'Somebody that I like',
            by: 'Kate East',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://d1csarkz8obe9u.cloudfront.net/posterpreviews/creative-music-album-cover-design-template-f4ce22c75f3fff9758bc01250abc6e05_screen.jpg?ts=1594215605',
            song: 'Memories',
            by: 'Anthony Knight',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://img.freepik.com/free-vector/electro-music-album_53876-67225.jpg?w=2000',
            song: 'Electronic',
            by: 'Electronic Music',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://d1csarkz8obe9u.cloudfront.net/posterpreviews/pink-cloud-cd-cover-music-design-template-258c703e9959b4635649e3944488c688_screen.jpg?ts=1631060402',
            song: 'CLOUD',
            by: 'Brian Sarubbi',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://pub-static.fotor.com/assets/projects/pages/55126b29-ff8d-475c-a5b5-d711e81caa6d/600w/purple-love-song-music-album-cover-64e5ec1b-0ed6-43a0-96e6-57a26534a584.jpg',
            song: 'Somebody that I like',
            by: 'Kate East',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://d1csarkz8obe9u.cloudfront.net/posterpreviews/creative-music-album-cover-design-template-f4ce22c75f3fff9758bc01250abc6e05_screen.jpg?ts=1594215605',
            song: 'Memories',
            by: 'Anthony Knight',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://img.freepik.com/free-vector/electro-music-album_53876-67225.jpg?w=2000',
            song: 'Electronic',
            by: 'Electronic Music',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://d1csarkz8obe9u.cloudfront.net/posterpreviews/pink-cloud-cd-cover-music-design-template-258c703e9959b4635649e3944488c688_screen.jpg?ts=1631060402',
            song: 'CLOUD',
            by: 'Brian Sarubbi',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://pub-static.fotor.com/assets/projects/pages/55126b29-ff8d-475c-a5b5-d711e81caa6d/600w/purple-love-song-music-album-cover-64e5ec1b-0ed6-43a0-96e6-57a26534a584.jpg',
            song: 'Somebody that I like',
            by: 'Kate East',
            releasedOn: '03/03/2023',
          },
          {
            url: 'https://d1csarkz8obe9u.cloudfront.net/posterpreviews/creative-music-album-cover-design-template-f4ce22c75f3fff9758bc01250abc6e05_screen.jpg?ts=1594215605',
            song: 'Memories',
            by: 'Anthony Knight',
            releasedOn: '03/03/2023',
          },
        ]"
      />
    </div>

    <div class="pb-40"></div>
  </div>
</template>

<script setup>
import MixesInspiredBy from "../components/MixesInspiredBy.vue";
import MultiArtistSelect from "../components/MultiArtistSelect.vue";
import CustomCarousel from "../components/CustomCarousel.vue";
import Highlights from "../components/Highlights.vue";
</script>
