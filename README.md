# Halooo 👋
![Anime Retro GIF](https://media.giphy.com/media/13HgwGsXF0aiGY/giphy.gif)

---

## About Me 🌟  
- 🎓 **Currently learning**: Backend development and data science (mostly backend).  
- 💻 **Skills**: Never Enough of Skills.  
- 🌱 **Hobbies**: Explore anything!  

---

## My GitHub Stats 📊  
Didnt know how to make a GitHub Stats    

---

> _"Singkat saja...... Paham !??"_  



import React from 'react';
import { View, Text, StyleSheet, Image, TouchableOpacity } from 'react-native';
import Footer from './footer';

const Profile = () => {
  return (
    <View style={styles.container}>
      {/* Background Image */}
      <Image
        source={require('../source/assets/img/profile/profile_team.jpg')} // Ganti dengan path gambar background Anda
        style={styles.backgroundImage}
      />

      {/* Profile Section */}
      <View style={styles.profileSection}>
        {/* Profile Picture */}
        <Image
          source={require('../source/assets/img/profile/profile_team.jpg')} // Ganti dengan path gambar profil Anda
          style={styles.profilePicture}
        />

        {/* Profile Button */}
        <Text style={styles.infoText}>Kelompok Satu</Text>
      </View>

      {/* User Information */}
      <View style={styles.infoSection}>
        <Text style={styles.infoText}>Nama 1</Text>
        <Text style={styles.infoText}>Nama 2</Text>
        <Text style={styles.infoText}>Nama 3</Text>
        <Text style={styles.infoText}>Nama 4</Text>
        <Text style={styles.infoText}>Nama 5</Text>
      </View>

      {/* Footer */}
      <Footer />
    </View>
  );
};

const styles = StyleSheet.create({
  container: {
    flex: 1,
    backgroundColor: '#fff',
  },
  backgroundImage: {
    width: '100%',
    height: 200,
    resizeMode: 'cover',
  },
  profileSection: {
    alignItems: 'center',
    marginTop: -50, // Untuk mengangkat bagian foto profil ke atas
  },
  profilePicture: {
    width: 100,
    height: 100,
    borderRadius: 50,
    borderWidth: 3,
    borderColor: '#fff',
  },
  profileButton: {
    marginTop: 10,
    backgroundColor: '#F3E9FF',
    paddingVertical: 8,
    paddingHorizontal: 16,
    borderRadius: 20,
  },
  profileButtonText: {
    color: '#7B61FF',
    fontSize: 14,
    fontWeight: 'bold',
  },
  infoSection: {
    alignItems: 'center',
    marginTop: 20,
  },
  infoText: {
    fontSize: 16,
    fontWeight: 'bold',
    marginVertical: 5,
    color: '#000',
  },
});

export default Profile;
