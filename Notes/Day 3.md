Day 3 - First Self-Hosted AI

Date: June 12, 2026

Objective

Install and test a locally hosted AI model using Ollama.

Accomplishments
Installed Ollama successfully on Arch Linux.
Learned that Ollama runs as a background service and is primarily accessed through the terminal.
Downloaded and launched my first local AI model.
Successfully interacted with the model through the command line.
Experiment

I asked the AI whether it could determine my computer's hardware specifications.

The model responded that it was a cloud-based AI hosted on remote servers and could not directly access my hardware.

This raised an interesting question: if the AI was actually running on my laptop, why did it believe it was hosted in the cloud?

To test this, I disconnected my laptop from the internet and asked the model:

Who is Naruto Uzumaki? Is this a real person or from a fictional universe?

The model correctly explained that Naruto Uzumaki is a fictional character from the Naruto manga and anime series.

What I Learned

The AI model does not actually know where it is running. It generates responses based on patterns learned during training.

Because many AI systems are cloud-hosted, the model often defaults to describing itself as a cloud-based AI even when it is running locally through Ollama.

The Naruto test demonstrated that the model was functioning without internet access and that its knowledge was stored within the model itself rather than being retrieved online.

Key Takeaway

AI models do not possess awareness of their environment. They generate text based on learned patterns and can sometimes make incorrect assumptions about themselves.

This experiment helped me better understand the difference between a model's training data and the actual environment in which it is running.

Next Steps
Explore additional Ollama models.
Learn how model size affects performance.
Install a graphical interface such as Open WebUI.
Continue learning self-hosted AI concepts.

day 3 continued
while attemtpting to get webui running to give ollama a more chatgpt like experience I had to give me user permission to use docker which needed a reboot.
while rebooting startplasma-wayland was not working. I tried it multiple times and attempted to troubleshoot on my own. After consulting with chatgpt I decided to just run the command again and it for some reason just decided to work.
I now have webui installed and localhost web server running. Ollama is definitely behind on its intelligence or its ability to give the illusion of intelligence. I mentioned being disconnected from the internet to me and I had to inform it that it was infact connected to the internet. It responded by saying I thought so!
Apon initial boot up of open webui I am very impressed with how similar to chatgpt it looks.
Open webui is unable to connect with ollama. This is not as straight forward as I thought it would be. But I guess nothing with Arch is. 
After much troubleshooting i got it working.
I once again disconnected from the internet and asked it a question about an anime and it sort of knew what I was talking about. It got some info right and made up the rest.

