# <a name="integrate-microsoft-graph-security-api-alerts-with-ibm-qradar-siem-using-azure-monitor"></a>Azure Monitor を使用して Microsoft Graph セキュリティ API の警告を IBM QRadar SIEM と統合する

Microsoft Graph セキュリティのプロバイダーは、単一の REST エンドポイント経由で管理できます。 このエンドポイントは、[Azure Monitor](https://docs.microsoft.com/en-us/azure/monitoring-and-diagnostics/) に構成でき、いくつかの SIEM 製品へのコネクタをサポートしています。 この記事の手順 1 と 2 の指示は、イベント ハブ経由での消費をサポートするすべての Azure Monitor のコネクタに言及しています。 この記事では、[QRadar](https://www.ibm.com/us-en/marketplace/ibm-qradar-siem) SIEM コネクターのエンド ツー エンドの統合について説明します。

統合プロセスは、以下の手順で構成されます。

1. [テナントへのセキュリティ警告を受診するように Azure のイベント ハブをセットアップする](#step-1-set-up-an-event-hubs-namespace-in-azure-to-receive-security-alerts-for-your-tenant)。
2. [テナントからイベント ハブへセキュリティ警告を送信するように Azure Monitor を構成する](#step-2-configure-azure-monitor-to-send-security-alerts-from-your-tenant-to-the-event-hub)。
3. [QRadar をダウンロードしてインストールし、セキュリティ警告を実行する](#step-3-download-and-install-the-qradar-to-consume-security-alerts)。

これらの手順を完了すると、IBM QRadar は、テナントがライセンスを供与されているすべての Microsoft Graph 統合セキュリティ製品から、セキュリティ警告を実行します。 ユーザーがライセンスを取得した新しいセキュリティ製品もこの接続を使用して同じスキーマで警告を送信するため、追加の統合作業は発生しません。

## <a name="step-1-set-up-an-event-hubs-namespace-in-azure-to-receive-security-alerts-for-your-tenant"></a>手順 1: テナントにセキュリティ警告を受診するように Azure の Event Hubs 名前空間をセットアップする

はじめに、[Microsoft Azure Event Hubs](https://docs.microsoft.com/en-us/azure/event-hubs/) の名前空間とイベント ハブを作成する必要があります。 この名前空間とイベント ハブは、組織のすべてのセキュリティ警告の送信先になります。 Event Hubs 名前空間は、同じアクセス ポリシーを共有するイベント ハブの論理的なグループです。 Event Hubs 名前空間とイベント ハブを作成するときは、以下の点に注意してください。

- 特に同じイベント ハブを介して他の Azure 監視データを送信する場合は、Standard Event Hubs 名前空間を使用することをお勧めします。
- 通常、必要なスループット ユニットは 1 つだけです。 使用量の増加に合わせてスケールアップする必要がある場合は、名前空間のスループット ユニットの数を後からいつでも手動で増やすことができ、自動インフレを有効にすることもできます。
- スループット ユニットの数によって、イベント ハブのスループットを増やすことができます。 パーティションの数によって、多くのコンシューマー間で使用量を並列化できます。 1 つのパーティションで最大 20 MBps (1 秒あたり約 20,000 メッセージ) に対応します。 データを使用するツールによっては、複数のパーティションからの使用がサポートされない場合があります。 設定するパーティションの数がわからない場合は、4 個のパーティションから始めることをお勧めします。
- イベント ハブでのメッセージのリテンション期間は、7 日間に設定することをお勧めします。 これにより、コンシューマー ツールの停止期間が 1 日を超えた場合でも、中断した時点 (最大 7 日前のイベントまで) をツールで選択できるようになります。
- イベント ハブの既定のコンシューマー グループを使用することをお勧めします。 2 つの異なるツールが同じイベント ハブの同じデータを使用しない限り、追加のコンシューマー グループを作成したり、別のコンシューマー グループを使用したりする必要はありません。
- 通常、イベント ハブのデータを使用するマシンのポート 5671 と 5672 を開く必要があります。

[Event Hubs のよく寄せられる質問](https://docs.microsoft.com/en-us/azure/event-hubs/event-hubs-faq)も参照してください。

1. [Azure Portal](https://portal.azure.com/) にログオンし、画面左上の **[リソースの作成]** を選択します。

    ![[リソースの作成] の画像](../concepts/images/create-resource.png)

2. **[モノのインターネット (IoT)]** を選択し、**[Event Hubs]** を選択します。

    ![[Event Hubs] の画像](../concepts/images/event-hubs.png)

3. **[名前空間の作成]** で、名前空間の名前を入力します。 名前空間の名前が使用できることを確認した後、価格レベル (Basic または Standard) を選択します。 さらに、Azure サブスクリプション、リソース グループ、およびリソースを作成する場所を選択します。 **[作成]** を選択して名前空間を作成します。 システムによるリソースのプロビジョニングが完了するまで、数分かかることがあります。

    ![[名前空間の作成] の画像](../concepts/images/create-namespace.png)

## <a name="step-2-configure-azure-monitor-to-send-security-alerts-from-your-tenant-to-the-event-hub"></a>手順 2: テナントからイベント ハブにセキュリティの警告を送信するように Azure Monitor を構成する

Azure Monitor を使った組織のセキュリティの警告のストリーミングを有効にする操作は、Azure Active Directory (Azure AD) テナント全体で 1 回だけ実行します。 Microsoft Graph セキュリティ API がライセンスされ有効になっているすべての製品では、実行しているアプリケーションにデータをストリーミングしながら、Azure Monitor にセキュリティ警告を送信し始めます。 所属組織がライセンスし展開した Microsoft Graph セキュリティ API が有効になっている追加の製品はすべて、この同じ Azure Monitor の構成を経由して、セキュリティ警告を自動的にストリーミングします。 組織による統合作業はそれ以上必要ありません。

セキュリティの警告は、通常は組織内のセキュリティ対応担当者と全体管理者だけが表示できる高い権限を持つデータです。 このため、テナントのセキュリティの警告と SIEM システムの統合を構成する手順では、Azure AD の全体管理者アカウントが必要です。 このアカウントは、セットアップ中に組織のセキュリティ警告を Azure Monitor に送信するよう要求するときに、1 回だけ必要になります。

> **注:** 現時点では、Azure Monitor の [診断設定] ブレードでは、テナント レベルのリソースの構成をサポートしていません。 Microsoft Graph セキュリティ API の警告はテナント レベルのリソースで、Azure のリソース マネージャーの API を使用して、組織のセキュリティの警告の消費をサポートするように、Azure Monitor を構成する必要があります。

1. Azure のサブスクリプション ([すべてのサービス] の下にあります) で、"microsoft.insights" (Azure Monitor) をリソース プロバイダとして登録します。  
> **注:** "Microsoft.SecurityGraph" (Microsoft Graph のセキュリティ API) は、前述のようにテナント レベルのリソースですので、Azure サブスクリプションのリソース プロバイダーとしては登録しないでください。 テナント レベルの構成は後述する #6 で扱います。

2. Azure Resource Manager API を使用して Azure Monitor を構成するには、[ARMClient](https://github.com/projectkudu/ARMClient) ツールを入手します。 このツールは、コマンド ラインから Azure Portal に REST API 呼び出しを送信するために使用されます。

3. 次のような診断設定要求の JSON ファイルを準備します。

    ``` json
    {
      "location": "",
      "properties": {
        "name": "securityApiAlerts",
        "serviceBusRuleId": "/subscriptions/SUBSCRIPTION_ID/resourceGroups/RESOURCE_GROUP/providers/Microsoft.EventHub/namespaces/EVENT_HUB_NAMESPACE/authorizationrules/RootManageSharedAccessKey",
        "logs": [
          {
            "category": "Alert",
            "enabled": true,
            "retentionPolicy": {
              "enabled": true,
              "days": 7
            }
          }
        ]
      }
    }
    ```

    JSON ファイル内の値を次のように置き換えます。

    **SUBSCRIPTION_ID** は、組織からセキュリティの警告を送信するときに使用するリソース グループとイベント ハブの名前空間をホストする Azure サブスクリプションのサブスクリプション ID です。

    **RESOURCE_GROUP** は、組織からセキュリティの警告を送信するときに使用するイベント ハブの名前空間を含むリソース グループです。

    **EVENT_HUB_NAMESPACE** は、組織からセキュリティの警告を送信するときに使用するイベント ハブの名前空間です。

    **“days”:** は、イベント ハブにメッセージを保持する日数です。

4. ARMClient.exe を起動するディレクトリに、このファイルを JSON 形式で保存します。 たとえば、ファイル名を **AzMonConfig.json** とします。

5. 次のコマンドを実行して ARMClient ツールにサインインします。 全体管理者アカウントの資格情報を使用する必要があります。

    ``` shell
    ARMClient.exe login
    ```

6. 次のコマンドを実行して、セキュリティの警告をイベント ハブの名前空間に送信するように Azure Monitor を構成します。 これにより、名前空間の内部にイベント ハブが自動的にプロビジョニングされ、セキュリティの警告のイベント ハブへのフローが開始されます。 設定名 (この例では **securityApiAlerts**) が JSON ファイルの **name** フィールドに設定した設定名と一致することを確認してください。

    ``` shell
    ARMClient.exe put https://management.azure.com/providers/Microsoft.SecurityGraph/diagnosticSettings/securityApiAlerts?api-version=2017-04-01-preview  @".\AzMonConfig.json"
    ```

7. 設定が正しく適用されていることを確認するには、次のコマンドを実行して、出力が JSON ファイルの設定と一致していることを確認します。

    ``` shell
    ARMClient.exe get https://management.azure.com/providers/Microsoft.SecurityGraph/diagnosticSettings/securityApiAlerts?api-version=2017-04-01-preview
    ```
8. ARMClient ツールを終了します。 これで、イベント ハブにテナントのセキュリティの警告を送信するための Azure Monitor の構成が完了しました。

## <a name="step-3-download-and-install-the-qradar-to-consume-security-alerts"></a>手順 3: QRadar をダウンロードしてインストールし、セキュリティ警告を実行する

1. [IBM QRadar](https://www.ibm.com/us-en/marketplace/ibm-qradar-siem) をダウンロードしてインストールします。 Microsoft Azure Event Hub からイベントを読み取るには、**Patch 7 付属のバージョン 7.2.8 またはそれ以降が必要**です。
2. 「[Microsoft Azure Event Hubs を構成して IBM QRadar と通信する](https://www.ibm.com/support/knowledgecenter/SS42VS_DSM/t_dsm_guide_microsoft_azure_enable_event_hubs.html)」の手順に従い、イベント ハブを構成します。
3. 最後に、「[QRadar を構成して、Microsoft Azure Event Hubs のプロトコルを使用して Microsoft Azure Event Hubs からイベントを収集する](https://www.ibm.com/support/knowledgecenter/SS42VS_DSM/t_logsource_microsoft_azure_event_hubs.html)」の手順に従い、セキュリティ警告の表示を開始します。
  
 > **注:** Microsoft Azure の IBM QRadar との統合では、「[Microsoft Azure DSM 仕様](https://www.ibm.com/support/knowledgecenter/SS42VS_DSM/c_dsm_guide_microsoft_azure_DSM_specs.html)」 に一覧表示されているイベントをサポートしています。 現在、Microsoft Graph セキュリティ API の警告に対する完全なサポートを追加するため、IBM QRadar と共同作業中です。 現時点では、Microsoft Graph セキュリティ API の警告を受診したら、IBM QRadar のコンソールで表示することができます。 [DSM エディター](https://www.ibm.com/support/knowledgecenter/SS42VS_7.2.8/com.ibm.qradar.doc/c_qradar_adm_dsm_ed_overview.html) を使用して、Microsoft Graph セキュリティ API の警告の解析を有効にできます。  
