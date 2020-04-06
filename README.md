# rn-use-interval

Using hooks to make an interval

# Installation

`npm i rn-use-interval --save`

# How to use
``````
const App = ()  => {
  const [time, setTime] = React.useState(0);
  useInterval(() => setTime(time+1), 1000);

  return (
      <>
        <SafeAreaView style={styles.container}>
          <Text>{time}</Text>
        </SafeAreaView>
      </>
  );
}

const styles = StyleSheet.create({
  container: {
    flex: 1,
    justifyContent: 'center',
    alignItems: 'center'
  }
});
``````


