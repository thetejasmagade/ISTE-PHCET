<template>
  <div class="bg-gray-900 mt-12 pb-8">
    <h1
      class="
        text-5xl
        font-extrabold
        text-transparent
        bg-clip-text bg-gradient-to-br
        from-yellow-400
        to-red-600
        pt-8
        text-center
      "
      style='Inter, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Fira Sans", "Droid Sans", "Helvetica Neue", sans-serif;'
    >
      Team
    </h1>
    <div>
      <p
        class="
          text-4xl
          font-extrabold
          text-transparent
          bg-clip-text bg-gradient-to-br
          from-pink-500
          to-yellow-500
          text-center
          font-normal
          pt-12
          pb-2
        "
      >
        Principal Sir
      </p>
      <div class="grid grid-cols-1 gap-8 md:grid-cols-3 px-4 pt-12">
        <div class=""></div>
        <TeamCard
          :name="data[0][0].name"
          :post="data[0][0].post"
          :description="data[0][0].description"
          :avatar="data[0][0].avatar"
          :email="data[0][0].email"
          :linkedin="data[0][0].linkedin"
        />
        <div class=""></div>
      </div>
      <p
        class="
          text-4xl
          font-extrabold
          text-transparent
          bg-clip-text bg-gradient-to-br
          from-pink-500
          to-yellow-500
          text-center
          font-normal
          pt-12
          pb-2
        "
      >
        Head Of Department
      </p>
      <div class="grid grid-cols-1 gap-8 md:grid-cols-3 px-4 pt-12">
        <div class=""></div>
        <TeamCard
          :name="data[0][1].name"
          :post="data[0][1].post"
          :description="data[0][1].description"
          :avatar="data[0][1].avatar"
          :email="data[0][1].email"
          :linkedin="data[0][1].linkedin"
        />
        <div class=""></div>
      </div>
      <p
        class="
          text-4xl
          font-extrabold
          text-transparent
          bg-clip-text bg-gradient-to-br
          from-pink-500
          to-yellow-500
          text-center
          font-normal
          pt-12
          pb-2
        "
      >
        Faculty Co-Ordinators
      </p>
      <div class="grid grid-cols-1 gap-8 md:grid-cols-2 px-4 md:px-52 pt-8">
        <TeamCard
          :name="data[1][0].name"
          :post="data[1][0].post"
          :description="data[1][0].description"
          :avatar="data[1][0].avatar"
          :email="data[1][0].email"
          :linkedin="data[1][0].linkedin"
        />
        <TeamCard
          :name="data[1][1].name"
          :post="data[1][1].post"
          :description="data[1][1].description"
          :avatar="data[1][1].avatar"
          :email="data[1][1].email"
          :linkedin="data[1][1].linkedin"
        />
      </div>
      <p
        class="
          text-4xl
          font-extrabold
          text-transparent
          bg-clip-text bg-gradient-to-br
          from-pink-500
          to-yellow-500
          text-center
          font-normal
          pt-12
          pb-2
        "
      >
        Presidents
      </p>
      <div class="grid grid-cols-1 gap-8 md:grid-cols-2 px-4 md:px-52 pt-8">
        <TeamCard
          :name="data[2][0].name"
          :post="data[2][0].post"
          :description="data[2][0].description"
          :avatar="data[2][0].avatar"
          :email="data[2][0].email"
        />
        <TeamCard
          :name="data[2][1].name"
          :post="data[2][1].post"
          :description="data[2][1].description"
          :avatar="data[2][1].avatar"
          :email="data[2][1].email"
        />
        <TeamCard
          :name="data[2][2].name"
          :post="data[2][2].post"
          :description="data[2][2].description"
          :avatar="data[2][2].avatar"
          :email="data[2][2].email"
        />
      </div>
      <p
        class="
          text-4xl
          font-extrabold
          text-transparent
          bg-clip-text bg-gradient-to-br
          from-pink-500
          to-yellow-500
          text-center
          font-normal
          pt-12
          pb-2
        "
      >
        Event Team
      </p>
      <div class="grid grid-cols-1 gap-8 md:grid-cols-2 px-4 md:px-52 pt-8">
        <TeamCard
          :name="data[3][0].name"
          :post="data[3][0].post"
          :description="data[3][0].description"
          :avatar="data[3][0].avatar"
          :email="data[3][0].email"
        />
        <TeamCard
          :name="data[3][1].name"
          :post="data[3][1].post"
          :description="data[3][1].description"
          :avatar="data[3][1].avatar"
          :email="data[3][1].email"
        />
        <TeamCard
          :name="data[3][2].name"
          :post="data[3][2].post"
          :description="data[3][2].description"
          :avatar="data[3][2].avatar"
          :email="data[3][2].email"
        />
        <TeamCard
          :name="data[3][3].name"
          :post="data[3][3].post"
          :description="data[3][3].description"
          :avatar="data[3][3].avatar"
          :email="data[3][3].email"
        />
        <TeamCard
          :name="data[3][4].name"
          :post="data[3][4].post"
          :description="data[3][4].description"
          :avatar="data[3][4].avatar"
          :email="data[3][4].email"
        />
      </div>

      <p
        class="
          text-4xl
          font-extrabold
          text-transparent
          bg-clip-text bg-gradient-to-br
          from-pink-500
          to-yellow-500
          text-center
          font-normal
          pt-12
          pb-2
        "
      >
        Event Team
      </p>
      <div class="grid grid-cols-1 gap-8 md:grid-cols-3 px-4 pt-12">
        <div class=""></div>
        <TeamCard
          :name="data[4][0].name"
          :post="data[4][0].post"
          :description="data[4][0].description"
          :avatar="data[4][0].avatar"
          :email="data[4][0].email"
        />
        <div class=""></div>
      </div>

      <p
        class="
          text-4xl
          font-extrabold
          text-transparent
          bg-clip-text bg-gradient-to-br
          from-pink-500
          to-yellow-500
          text-center
          font-normal
          pt-12
          pb-2
        "
      >
        Social Media
      </p>
      <div class="grid grid-cols-1 gap-8 md:grid-cols-3 px-4 pt-12">
        <div class=""></div>
        <TeamCard
          :name="data[5][0].name"
          :post="data[5][0].post"
          :description="data[5][0].description"
          :avatar="data[5][0].avatar"
          :email="data[5][0].email"
        />
        <div class=""></div>
      </div>

      <p
        class="
          text-4xl
          font-extrabold
          text-transparent
          bg-clip-text bg-gradient-to-br
          from-pink-500
          to-yellow-500
          text-center
          font-normal
          pt-12
          pb-2
        "
      >
        Technical Team
      </p>
      <div class="grid grid-cols-1 gap-8 md:grid-cols-2 px-4 md:px-52 pt-8">
        <TeamCard
          :name="data[6][0].name"
          :post="data[6][0].post"
          :description="data[6][0].description"
          :avatar="data[6][0].avatar"
          :email="data[6][0].email"
        />
        <TeamCard
          :name="data[6][1].name"
          :post="data[6][1].post"
          :description="data[6][1].description"
          :avatar="data[6][1].avatar"
          :email="data[6][1].email"
        />
      </div>

      <p
        class="
          text-4xl
          font-extrabold
          text-transparent
          bg-clip-text bg-gradient-to-br
          from-pink-500
          to-yellow-500
          text-center
          font-normal
          pt-12
          pb-2
        "
      >
        Graphics Team
      </p>
      <div class="grid grid-cols-1 gap-8 md:grid-cols-2 px-4 md:px-52 pt-8">
        <TeamCard
          :name="data[7][0].name"
          :post="data[7][0].post"
          :description="data[7][0].description"
          :avatar="data[7][0].avatar"
          :email="data[7][0].email"
        />
        <TeamCard
          :name="data[7][1].name"
          :post="data[7][1].post"
          :description="data[7][1].description"
          :avatar="data[7][1].avatar"
          :email="data[7][1].email"
        />
        <TeamCard
          :name="data[7][2].name"
          :post="data[7][2].post"
          :description="data[7][2].description"
          :avatar="data[7][2].avatar"
          :email="data[7][2].email"
        />
        <TeamCard
          :name="data[7][3].name"
          :post="data[7][3].post"
          :description="data[7][3].description"
          :avatar="data[7][3].avatar"
          :email="data[7][3].email"
        />
      </div>

      <p
        class="
          text-4xl
          font-extrabold
          text-transparent
          bg-clip-text bg-gradient-to-br
          from-pink-500
          to-yellow-500
          text-center
          font-normal
          pt-12
          pb-2
        "
      >
        Photography Team
      </p>
      <div class="grid grid-cols-1 gap-8 md:grid-cols-3 px-4 pt-12">
        <div class=""></div>
        <TeamCard
          :name="data[8][0].name"
          :post="data[8][0].post"
          :description="data[8][0].description"
          :avatar="data[8][0].avatar"
          :email="data[8][0].email"
        />
        <div class=""></div>
      </div>

      <p
        class="
          text-4xl
          font-extrabold
          text-transparent
          bg-clip-text bg-gradient-to-br
          from-pink-500
          to-yellow-500
          text-center
          font-normal
          pt-12
          pb-2
        "
      >
        Web Development Team
      </p>
      <div class="grid grid-cols-1 gap-8 md:grid-cols-2 px-4 md:px-52 pt-8">
        <TeamCard
          :name="data[9][0].name"
          :post="data[9][0].post"
          :description="data[9][0].description"
          :avatar="data[9][0].avatar"
          :email="data[9][0].email"
        />
        <TeamCard
          :name="data[9][1].name"
          :post="data[9][1].post"
          :description="data[9][1].description"
          :avatar="data[9][1].avatar"
          :email="data[9][1].email"
        />
      </div>

      <p
        class="
          text-4xl
          font-extrabold
          text-transparent
          bg-clip-text bg-gradient-to-br
          from-pink-500
          to-yellow-500
          text-center
          font-normal
          pt-12
          pb-2
        "
      >
        Publicity Team
      </p>
      <div class="grid grid-cols-1 gap-8 md:grid-cols-2 px-4 md:px-52 pt-8">
        <TeamCard
          :name="data[10][0].name"
          :post="data[10][0].post"
          :description="data[10][0].description"
          :avatar="data[10][0].avatar"
          :email="data[10][0].email"
        />
        <TeamCard
          :name="data[10][1].name"
          :post="data[10][1].post"
          :description="data[10][1].description"
          :avatar="data[10][1].avatar"
          :email="data[10][1].email"
        />
        <TeamCard
          :name="data[10][2].name"
          :post="data[10][2].post"
          :description="data[10][2].description"
          :avatar="data[10][2].avatar"
          :email="data[10][2].email"
        />
        <TeamCard
          :name="data[10][3].name"
          :post="data[10][3].post"
          :description="data[10][3].description"
          :avatar="data[10][3].avatar"
          :email="data[10][3].email"
        />
        <TeamCard
          :name="data[10][4].name"
          :post="data[10][4].post"
          :description="data[10][4].description"
          :avatar="data[10][4].avatar"
          :email="data[10][4].email"
        />
      </div>
      <p
        class="
          text-4xl
          font-extrabold
          text-transparent
          bg-clip-text bg-gradient-to-br
          from-pink-500
          to-yellow-500
          text-center
          font-normal
          pt-12
          pb-2
        "
      >
        Treasurer Team
      </p>
      <div class="grid grid-cols-1 gap-8 md:grid-cols-2 px-4 md:px-52 pt-8">
        <TeamCard
          :name="data[11][0].name"
          :post="data[11][0].post"
          :description="data[11][0].description"
          :avatar="data[11][0].avatar"
          :email="data[11][0].email"
        />
        <TeamCard
          :name="data[11][1].name"
          :post="data[11][1].post"
          :description="data[11][1].description"
          :avatar="data[11][1].avatar"
          :email="data[11][1].email"
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      data: [
        [
          {
            name: "Dr. Jagdish W. Bakal",
            post: "Principal",
            description:
              "Dr. J. W. Bakal, Principal PHCET and a great support for us. Dr. Bakal has 32 years of Industry and Academic experience. He has already 7 Patents on his credit and has published more than 100 papers in International Journals",
            avatar:
              "https://phcet.ac.in/wp-content/uploads/2021/11/Dr.-Jagdish-Bakal-1.jpg",
            email: "mailto:jwbakal@mes.ac.in",
            linkedin: "https://in.linkedin.com/in/jagdish-bakal0508",
          },
          {
            name: "Dr. Divya Y. Chirayil",
            post: "Head Of Department",
            description:
              "Dr. D. Y. Chirayil has total 20 years of Teaching and Academic experience. She is the member of syllabus revision committiee for the UG program in IT Engineering. She has more than 23 International Conference and Journal Research Publication and 3 Patents to her credit.",
            avatar:
              "https://phcet.ac.in/wp-content/uploads/2020/04/Dr.-Divya-Chirayil.jpg",
            email: "mailto:dchirayil@mes.ac.in",
            linkedin: "https://www.linkedin.com/in/divya-chirayil-4754141a6/",
          },
        ],
        [
          {
            name: "Mr. Siddhesh Khanvilkar",
            post: "Faculty Co-Ordinator",
            description: "IT Department",
            avatar: "",
            email: "mailto:",
          },
          {
            name: "Ms. Rupali Sathe",
            post: "Faculty Co-Ordinator",
            description: "IT Department",
            avatar: "",
            email: "mailto:",
          },
        ],
        [
          {
            name: "Nitish Shetty",
            post: "President",
            description: "IT Department",
            avatar:
              "https://raw.githubusercontent.com/thetejasmagade/ace-team-images/master/nitish.jpg",
            email: "mailto:nitishnash19iteng@student.mes.ac.in",
          },
          {
            name: "Ankita Pattnaik",
            post: "Vice President",
            description: "IT Department",
            avatar:
              "https://raw.githubusercontent.com/thetejasmagade/ace-team-images/master/aakanksha.jpg",
            email: "mailto:ankitasp20iteng@student.mes.ac.in",
          },
          {
            name: "Rutuja Kore",
            post: "Vice President",
            description: "IT Department",
            avatar:
              "https://csi.phcet.ac.in/static/media/publicity-team-member-3.18d85322.png",
            email: "mailto:rutujautko19iteng@student.mes.ac.in",
          },
        ],
        [
          {
            name: "Avishkar Vichare",
            post: "Event Head Co-Ordinator",
            description: "IT Department",
            avatar: "",
            email: "mailto:",
          },
          {
            name: "Amruta Padyal",
            post: "Event Head Co-Ordinator",
            description: "IT Department",
            avatar: "",
            email: "mailto:",
          },
          {
            name: "Khushnuma Mujavar",
            post: "Event Co-Ordinator",
            description: "IT Department",
            avatar: "",
            email: "mailto:",
          },
          {
            name: "Gaurav Parab",
            post: "Event Co-Ordinator",
            description: "IT Department",
            avatar: "",
            email: "mailto:",
          },
          {
            name: "Ankita Mhatre",
            post: "Event Co-Ordinator",
            description: "IT Department",
            avatar: "",
            email: "mailto:",
          },
        ],
        [
          {
            name: "Anamika Zagade",
            post: "Content Head",
            description: "IT Department",
            avatar: "",
            email: "mailto:",
          },
        ],
        [
          {
            name: "Hritik Gole",
            post: "Social Media Head",
            description: "IT Department",
            avatar: "",
            email: "mailto:",
          },
        ],
        [
          {
            name: "Pritish Parkar",
            post: "Technical Head",
            description: "IT Department",
            avatar: "",
            email: "mailto:",
          },
          {
            name: "Shubham Gajarushi",
            post: "Technical Co-Ordinator",
            description: "IT Department",
            avatar: "",
            email: "mailto:",
          },
        ],
        [
          {
            name: "Nishant Patil",
            post: "Graphics Head",
            description: "IT Department",
            avatar: "",
            email: "mailto:",
          },
          {
            name: "Shubham Mahto",
            post: "Graphics Co-Ordinator",
            description: "IT Department",
            avatar: "",
            email: "mailto:",
          },
          {
            name: "Gaurav Madhavi",
            post: "Graphics Co-Ordinator",
            description: "IT Department",
            avatar: "",
            email: "mailto:",
          },
          {
            name: "Vikrant Ahir",
            post: "Graphics Co-Ordinator",
            description: "IT Department",
            avatar: "",
            email: "mailto:",
          },
        ],
        [
          {
            name: "Hrushikesh Tambe",
            post: "Photography Head",
            description: "IT Department",
            avatar: "",
            email: "mailto:",
          },
        ],
        [
          {
            name: "Rabee Shaikh",
            post: "Website Development Head",
            description: "IT Department",
            avatar: "",
            email: "mailto:",
          },
          {
            name: "Tejas Magade",
            post: "Website Developer",
            description: "IT Department",
            avatar: "",
            email: "mailto:",
          },
        ],
        [
          {
            name: "Shubham Patil",
            post: "Publicity Head",
            description: "IT Department",
            avatar: "",
            email: "mailto:",
          },
          {
            name: "Aadarsh Poojary",
            post: "Publicity Head",
            description: "IT Department",
            avatar: "",
            email: "mailto:",
          },
          {
            name: "Antima Yadav",
            post: "Publicity Co-Ordinator",
            description: "IT Department",
            avatar: "",
            email: "mailto:",
          },
          {
            name: "Harshala Patil",
            post: "Publicity Co-Ordinator",
            description: "IT Department",
            avatar: "",
            email: "mailto:",
          },
          {
            name: "Dnyaneshwari Hande",
            post: "Publicity Co-Ordinator",
            description: "IT Department",
            avatar: "",
            email: "mailto:",
          },
        ],
        [
          {
            name: "Shubham Patil",
            post: "Treasurer Head",
            description: "IT Department",
            avatar: "",
            email: "mailto:",
          },
          {
            name: "Prerna Vishwasrao",
            post: "Treasurer Co-Ordinator",
            description: "IT Department",
            avatar: "",
            email: "mailto:",
          },
        ],
      ],
    };
  },
};
</script>

<style>
</style>