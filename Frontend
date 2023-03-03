import React, { useState } from 'react';

function App() {
  const [selectedTopics, setSelectedTopics] = useState([]);

  const handleTopicSelection = (event) => {
    const topic = event.target.value;
    const index = selectedTopics.indexOf(topic);

    if (index === -1) {
      setSelectedTopics([...selectedTopics, topic]);
    } else {
      const newSelectedTopics = [...selectedTopics];
      newSelectedTopics.splice(index, 1);
      setSelectedTopics(newSelectedTopics);
    }
  };

  return (
    <div>
      <h1>Employee Notifications</h1>
      <div>
        <h2>Select topics to subscribe to:</h2>
        <label>
          <input type="checkbox" value="topic1" onChange={handleTopicSelection} />
          Topic 1
        </label>
        <label>
          <input type="checkbox" value="topic2" onChange={handleTopicSelection} />
          Topic 2
        </label>
        <label>
          <input type="checkbox" value="topic3" onChange={handleTopicSelection} />
          Topic 3
        </label>
        <label>
          <input type="checkbox" value="topic4" onChange={handleTopicSelection} />
          Topic 4
        </label>
      </div>
      <div>
        <h2>Notifications:</h2>
        <p>Notifications will appear here when new messages are published for the topics you subscribed to.</p>
      </div>
    </div>
  );
}

export default App;
