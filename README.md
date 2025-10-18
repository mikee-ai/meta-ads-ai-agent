# 🤖 Master Meta Ads AI Agent

This autonomous AI agent is designed to be your expert Meta Ads Media Buyer. It leverages the principles from the Meta Media Buying Master (MBM) course to automatically generate, test, and optimize video ad campaigns.

## ✨ Features

- **Autonomous Operation**: The agent handles the entire campaign lifecycle, from creative generation to ad launch and optimization.
- **AI-Powered Creative**: Utilizes state-of-the-art AI models (Flux Pro for images, Hailuo 2 for video) to generate high-quality, cost-effective ad creatives.
- **MBM Strategy Integration**: Implements the micro-budget testing, avatar-first, and data-driven optimization strategies from the MBM course.
- **Cost-Effective**: Creates complete video ads for approximately **$0.14 each**, a 93% cost savings compared to other high-end models like Veo 3.1.
- **Scalable**: Designed to test dozens of ad variations and automatically scale the winners.

## 🚀 How to Use

The agent is deployed on your VPS at `31.97.145.136` in the `/root/` directory.

### **1. Connect to Your VPS**

```bash
ssh root@31.97.145.136
```

### **2. Navigate to the Agent Directory**

```bash
cd /root
```

### **3. Run the Agent**

To generate a new campaign with a specific number of ad variations, run the script with the number of variations as an argument.

**Example: Generate a campaign with 5 ad variations**

```bash
python3 master_meta_ads_agent.py 5
```

This will create a new campaign with 5 different ad sets, each with its own unique video ad, for a total ad spend of $25/day ($5/day per ad set).

### **4. Monitor Performance**

- The agent will print a link to the campaign in Meta Ads Manager.
- Monitor the performance of the ads for 48-72 hours.
- The agent is designed to follow the MBM principles of pausing ads with a CTR below 1% and scaling the budget of winning ads. (This functionality can be fully automated in the next version).

## 🔧 Customization

You can customize the creative concepts and mascot description by editing the `master_meta_ads_agent.py` file.

- **Mascot Description**: Modify the `self.mascot_desc` variable to change the appearance of the AI-generated mascot.
- **Creative Concepts**: Add, remove, or edit the dictionaries in the `self.creative_concepts` list to test different benefits, ad copy, and headlines.

## 📈 Next Steps & Future Development

- **Full Automation**: The agent can be extended to run on a schedule (e.g., daily) to continuously generate new creatives and optimize campaigns.
- **Performance Dashboard**: A web-based dashboard can be built to visualize campaign performance and ROI.
- **Advanced Optimization**: Integrate more advanced optimization logic, such as automatically duplicating winning ad sets and increasing their budgets.
- **SaaS Platform**: This entire system can be packaged into a SaaS platform for other businesses to use, creating a new revenue stream.

