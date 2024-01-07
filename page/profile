import React from "react";
import {
  View,
  FlatList,
  Image,
  Text,
  StyleSheet,
  Dimensions,
} from "react-native";

const { width } = Dimensions.get("window");
const imageWidth = width / 3; // Assuming you want 3 images per row

const imageUrls = [
  "https://d1vbn70lmn1nqe.cloudfront.net/prod/wp-content/uploads/2023/07/13073811/Praktis-dengan-Bahan-Sederhana-Ini-Resep-Nasi-Goreng-Special-1.jpg.webp",
  "https://www.frisianflag.com/storage/app/media/uploaded-files/nasi-kuning-ricecooker.jpg",
  "https://www.ambitiouskitchen.com/wp-content/uploads/2021/10/Slow-Cooker-White-Wine-Chicken-Stew-7.jpg",
  "https://www.astronauts.id/blog/wp-content/uploads/2023/03/Resep-Rendang-Daging-Sapi-Untuk-Lebaran-Gurih-dan-Nikmat-1024x683.jpg",
  "https://cdn.loveandlemons.com/wp-content/uploads/2023/02/vegetarian-pizza.jpg",
  "https://www.thecookierookie.com/wp-content/uploads/2023/04/featured-stovetop-burgers-recipe.jpg",
  "https://awsimages.detik.net.id/community/media/visual/2023/03/14/resep-rawon-daging-surabaya_43.jpeg?w=650&amp;q=80",
  "https://www.unileverfoodsolutions.co.id/dam/global-ufs/mcos/SEA/calcmenu/recipes/ID-recipes/soups/soto-betawi/main-header.jpg",
  "https://i0.wp.com/resepkoki.id/wp-content/uploads/2017/05/Resep-Sup-Konro.jpg?fit=1893%2C1920&amp;ssl=1",
  "https://www.frisianflag.com/storage/app/media/uploaded-files/nasi-kuning-ricecooker.jpg",
  "https://www.ambitiouskitchen.com/wp-content/uploads/2021/10/Slow-Cooker-White-Wine-Chicken-Stew-7.jpg",
  "https://www.astronauts.id/blog/wp-content/uploads/2023/03/Resep-Rendang-Daging-Sapi-Untuk-Lebaran-Gurih-dan-Nikmat-1024x683.jpg",
  // Add more image URLs as needed
];

const renderImageItem = ({ item }) => (
  <Image style={styles.image} source={{ uri: item }} resizeMode="cover" />
);

const App = () => {
  const renderHeader = () => (
    <View style={styles.header}>
      <View style={styles.headerColumn1}>
        <Image
          style={styles.profileImage}
          source={{
            uri: "https://i0.wp.com/resepkoki.id/wp-content/uploads/2017/05/Resep-Sup-Konro.jpg?fit=1893%2C1920&amp;ssl=1",
          }}
        />
      </View>
      <View style={styles.headerColumn2}>
        <Text style={styles.nameText}>Your Name</Text>
        <Text style={styles.statsText}>
          5 posts 100 followers 100 following
        </Text>
        <Text style={styles.additionalText}>
          Lorem ipsum dolor sit amet consectetur. Haretra id a olor a eu. Sed
          duis erat orci tortor varius dignissim. Facsili de ouir.
        </Text>
      </View>
    </View>
  );

  return (
    <View style={styles.container}>
      <FlatList
        data={imageUrls}
        renderItem={renderImageItem}
        keyExtractor={(item, index) => index.toString()}
        numColumns={3} // Number of images per row
        ListHeaderComponent={renderHeader}
      />
    </View>
  );
};

const styles = StyleSheet.create({
  container: {
    flex: 1,
  },
  header: {
    flexDirection: "row",
    padding: 16,
    borderBottomColor: "#ddd",
    borderBottomWidth: 1,
  },
  headerColumn1: {
    flex: 1,
    alignItems: "center",
  },
  headerColumn2: {
    flex: 2,
    marginLeft: 16,
  },
  profileImage: {
    width: 80,
    height: 80,
    borderRadius: 40,
  },
  nameText: {
    fontSize: 18,
    fontWeight: "bold",
  },
  statsText: {
    marginTop: 8,
    color: "#555",
  },
  additionalText: {
    marginTop: 8,
    color: "#777",
  },
  image: {
    width: imageWidth,
    height: imageWidth,
    margin: 2, // Adjust the margin as needed
  },
});

export default App;
