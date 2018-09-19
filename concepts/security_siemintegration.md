# <a name="integrate-microsoft-graph-security-api-alerts-with-a-siem"></a>Microsoft グラフ セキュリティ API の警告と SIEM の統合

Microsoft グラフ セキュリティ API により、Microsoft Graph のセキュリティ プロバイダーとして知られるすべてのマイクロソフトのセキュリティ製品からのセキュリティの警告を、単一の REST エンドポイントを通じて管理できるようになります。組織によっては、Azure 固有のログ データを、既に Azure モニターを通じて SIEM ソリューションに取り込んでいる可能性があります。統合を簡単にするために、Microsoft Graph  セキュリティ API を通じて使用可能なセキュリティの警告も、Azure モニターを介して、お客様がサブスクリプション用に準備することができます。組織が既に Azure モニター統合を SIEM ソリューションを用いて構成している場合 は、Azure モニターを通じて使用可能な既存のデータに加えて、組織のセキュリティの警告も、今や簡単にストリーミングすることができます。

Azure  Monitor は、いくつかの SIEM 製品へのコネクタをサポートしています。 サポートされている SIEM 製品の一覧は、「[監視データをイベント ハブへ送信](https://docs.microsoft.com/en-us/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub)」をご覧ください。 Microsoft Graph セキュリティ API の統合は現在、[Splunk](https://splunkbase.splunk.com/) と [QRadar](https://www.ibm.com/us-en/marketplace/ibm-qradar-siem) で使用できます。

 特定の SIEM ソリューションの Microsoft Graph セキュリティ API の統合については、以下をご覧ください。

- [Splunk](security-splunk-siemintegration.md)
- [QRadar](security-qradar-siemintegration.md)
