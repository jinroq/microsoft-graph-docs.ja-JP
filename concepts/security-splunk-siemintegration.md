---
title: Azure Monitor を使った Microsoft Graph セキュリティ API の警告と SIEM の統合
description: Microsoft Graph Security プロバイダーは、単一の REST エンドポイントを通じて管理できます。 このエンドポイントは、複数の SIEM 製品へのコネクタをサポートする Azure Monitor に対して構成できます。 この記事の手順 1 と手順 2 は、イベント ハブを介した使用をサポートするすべての Azure Monitor コネクタに関係しています。 この記事では、Splunk SIEM コネクタのエンド ツー エンドの統合について説明します。
ms.openlocfilehash: bdd1d1e192a4945c67727d20e594006a387fb156
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092477"
---
# <a name="integrate-microsoft-graph-security-api-alerts-with-your-siem-using-azure-monitor"></a><span data-ttu-id="05946-106">Azure Monitor を使った Microsoft Graph セキュリティ API の警告と SIEM の統合</span><span class="sxs-lookup"><span data-stu-id="05946-106">Integrate security API alerts with your SIEM using Azure Monitor</span></span>

<span data-ttu-id="05946-107">Microsoft Graph Security プロバイダーは、単一の REST エンドポイントを通じて管理できます。</span><span class="sxs-lookup"><span data-stu-id="05946-107">The Microsoft Graph Security providers can be managed through a single REST endpoint.</span></span> <span data-ttu-id="05946-108">このエンドポイントは、複数の SIEM 製品へのコネクタをサポートする [Azure Monitor](https://docs.microsoft.com/ja-JP/azure/monitoring-and-diagnostics/) に対して構成できます。</span><span class="sxs-lookup"><span data-stu-id="05946-108">This endpoint can be configured to [Azure Monitor](https://docs.microsoft.com/ja-JP/azure/monitoring-and-diagnostics/) which supports connectors to several SIEM products.</span></span> <span data-ttu-id="05946-109">この記事の手順 1 と手順 2 は、イベント ハブを介した使用をサポートするすべての Azure Monitor コネクタに関係しています。</span><span class="sxs-lookup"><span data-stu-id="05946-109">The instructions in Steps 1 and 2 of this article refer to all Azure Monitor connectors that support consumption via event hubs.</span></span> <span data-ttu-id="05946-110">この記事では、[Splunk](https://splunkbase.splunk.com/) SIEM コネクタのエンド ツー エンドの統合について説明します。</span><span class="sxs-lookup"><span data-stu-id="05946-110">This article describes the end-to-end configuration for the Splunk SIEM connector.</span></span>

<span data-ttu-id="05946-111">この統合プロセスは、以下の手順から構成されます。</span><span class="sxs-lookup"><span data-stu-id="05946-111">The integration process involves the following steps:</span></span>

1. [<span data-ttu-id="05946-112">テナントのセキュリティ警告を受信するように Azure イベント ハブをセットアップする</span><span class="sxs-lookup"><span data-stu-id="05946-112">Set up Azure your event hub to receive security alerts for your tenant</span></span>](#step-1-set-up-an-event-hubs-namespace-in-azure-to-receive-security-alerts-for-your-tenant)
2. [<span data-ttu-id="05946-113">テナントからイベント ハブにセキュリティ警告を送信するように Azure Monitor を構成する</span><span class="sxs-lookup"><span data-stu-id="05946-113">Configure Azure Monitor to send security alerts from your tenant to the event hub</span></span>](#step-2-configure-azure-monitor-to-send-security-alerts-from-your-tenant-to-the-event-hub)
3. [<span data-ttu-id="05946-114">Splunk がセキュリティの警告を使用できるように Splunk 向けの Azure Monitor アドオンをダウンロードしてインストールする</span><span class="sxs-lookup"><span data-stu-id="05946-114">Download and install the Azure Monitor Add-on for Splunk which will allow Splunk to consume security alerts</span></span>](#step-3-download-and-install-the-azure-monitor-add-on-for-splunk-which-will-allow-splunk-to-consume-security-alerts)
4. [<span data-ttu-id="05946-115">Splunk がイベント ハブからの読み取りに使用するアプリケーションをテナントの Azure Active Directory に登録する</span><span class="sxs-lookup"><span data-stu-id="05946-115">Register an application with your tenant Azure Active Directory which Splunk will use to read from the event hub</span></span>](#step-4-register-an-application-with-your-tenant-azure-active-directory-which-splunk-will-use-to-read-from-the-event-hub )
5. [<span data-ttu-id="05946-116">イベント ハブのアクセス キーを格納する Azure Key Vault を作成する</span><span class="sxs-lookup"><span data-stu-id="05946-116">Create an Azure Key vault to store the access key for the event hub</span></span>](#step-5-create-an-azure-key-vault-to-store-the-access-key-for-the-event-hub)
6. [<span data-ttu-id="05946-117">イベント ハブに格納されているセキュリティの警告を使用するように Splunk のデータ入力を構成する</span><span class="sxs-lookup"><span data-stu-id="05946-117">Configure the Splunk data inputs to consume security alerts stored in the event hub</span></span>](#step-6-configure-the-splunk-data-inputs-to-consume-security-alerts-stored-in-the-event-hub)

<span data-ttu-id="05946-118">上記の手順を完了すると、Splunk Enterprise はテナントにライセンスされたすべての Microsoft Graph 統合セキュリティ製品から出力されるセキュリティの警告を使用します。</span><span class="sxs-lookup"><span data-stu-id="05946-118">After you complete these steps, your Splunk Enterprise will consume security alerts from all the Microsoft Graph integrated security products for which your tenant is licensed.</span></span> <span data-ttu-id="05946-119">ユーザーがライセンスを取得した新しいセキュリティ製品もこの接続を使用して同じスキーマで警告を送信するため、追加の統合作業は発生しません。</span><span class="sxs-lookup"><span data-stu-id="05946-119">Any new security products that you license will also send alerts through this connection, in the same schema with no further integration work needed.</span></span>

## <a name="step-1-set-up-an-event-hubs-namespace-in-azure-to-receive-security-alerts-for-your-tenant"></a><span data-ttu-id="05946-120">手順 1: テナントのセキュリティ警告を受信するように Azure の Event Hubs 名前空間をセットアップする</span><span class="sxs-lookup"><span data-stu-id="05946-120">Step 1: Set up an Event Hubs namespace in Azure to receive security alerts for your tenant</span></span>

<span data-ttu-id="05946-121">最初に、[Microsoft Azure Event Hubs](https://docs.microsoft.com/ja-JP/azure/event-hubs/) 名前空間とイベント ハブを作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="05946-121">To begin, you need to create a Microsoft Azure Event Hubs namespace and event hub.</span></span> <span data-ttu-id="05946-122">この名前空間とイベント ハブは、組織のすべてのセキュリティ警告の送信先になります。</span><span class="sxs-lookup"><span data-stu-id="05946-122">This namespace and event hub is the destination for all your organization’s security alerts.</span></span> <span data-ttu-id="05946-123">Event Hubs 名前空間は、同じアクセス ポリシーを共有するイベント ハブの論理的なグループです。</span><span class="sxs-lookup"><span data-stu-id="05946-123">An Event Hubs namespace is a logical grouping of event hubs that share the same access policy.</span></span> <span data-ttu-id="05946-124">Event Hubs 名前空間とイベント ハブを作成するときは、以下の点に注意してください。</span><span class="sxs-lookup"><span data-stu-id="05946-124">Note a few details about the Event Hubs namespace and event hubs that you create:</span></span>

- <span data-ttu-id="05946-125">特に同じイベント ハブを介して他の Azure 監視データを送信する場合は、Standard Event Hubs 名前空間を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="05946-125">We recommend using a Standard Event Hubs namespace, particularly if you are sending other Azure monitoring data through these same event hubs.</span></span>
- <span data-ttu-id="05946-126">通常、必要なスループット ユニットは 1 つだけです。</span><span class="sxs-lookup"><span data-stu-id="05946-126">Typically, only one throughput unit is necessary.</span></span> <span data-ttu-id="05946-127">使用量の増加に合わせてスケールアップする必要がある場合は、名前空間のスループット ユニットの数を後からいつでも手動で増やすことができ、自動インフレを有効にすることもできます。</span><span class="sxs-lookup"><span data-stu-id="05946-127">If you need to scale up as your usage increases, you can always manually increase the number of throughput units for the namespace later or enable auto inflation.</span></span>
- <span data-ttu-id="05946-128">スループット ユニットの数によって、イベント ハブのスループットを増やすことができます。</span><span class="sxs-lookup"><span data-stu-id="05946-128">The number of throughput units allows you to increase throughput scale for your event hubs.</span></span> <span data-ttu-id="05946-129">パーティションの数によって、多くのコンシューマー間で使用量を並列化できます。</span><span class="sxs-lookup"><span data-stu-id="05946-129">The number of partitions allows you to parallelize consumption across many consumers.</span></span> <span data-ttu-id="05946-130">1 つのパーティションで最大 20 MBps (1 秒あたり約 20,000 メッセージ) に対応します。</span><span class="sxs-lookup"><span data-stu-id="05946-130">A single partition can do up to 20MBps, or approximately 20,000 messages per second.</span></span> <span data-ttu-id="05946-131">データを使用するツールによっては、複数のパーティションからの使用がサポートされない場合があります。</span><span class="sxs-lookup"><span data-stu-id="05946-131">Depending on the tool consuming the data, it may or may not support consuming from multiple partitions.</span></span> <span data-ttu-id="05946-132">設定するパーティションの数がわからない場合は、4 個のパーティションから始めることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="05946-132">If you're not sure about the number of partitions to set, we recommend starting with four partitions.</span></span>
- <span data-ttu-id="05946-133">イベント ハブでのメッセージのリテンション期間は、7 日間に設定することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="05946-133">We recommend that you set message retention on your event hub to 7 days.</span></span> <span data-ttu-id="05946-134">これにより、コンシューマー ツールの停止期間が 1 日を超えた場合でも、中断した時点 (最大 7 日前のイベントまで) をツールで選択できるようになります。</span><span class="sxs-lookup"><span data-stu-id="05946-134">If your consuming tool goes down for more than a day, this ensures that the tool can pick up where it left off (for events up to 7 days old).</span></span>
- <span data-ttu-id="05946-135">イベント ハブの既定のコンシューマー グループを使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="05946-135">We recommend using the default consumer group for your event hub.</span></span> <span data-ttu-id="05946-136">2 つの異なるツールが同じイベント ハブの同じデータを使用しない限り、追加のコンシューマー グループを作成したり、別のコンシューマー グループを使用したりする必要はありません。</span><span class="sxs-lookup"><span data-stu-id="05946-136">You don't need to create other consumer groups or use a separate consumer group unless you plan to have two different tools consume the same data from the same event hub.</span></span>
- <span data-ttu-id="05946-137">通常、イベント ハブのデータを使用するマシンのポート 5671 と 5672 を開く必要があります。</span><span class="sxs-lookup"><span data-stu-id="05946-137">Typically, port 5671 and 5672 must be opened on the machine consuming data from the event hub.</span></span>

<span data-ttu-id="05946-138">[Event Hubs のよく寄せられる質問](https://docs.microsoft.com/ja-JP/azure/event-hubs/event-hubs-faq)も参照してください。</span><span class="sxs-lookup"><span data-stu-id="05946-138">Also see the [Azure Event Hubs FAQ](https://docs.microsoft.com/ja-JP/azure/event-hubs/event-hubs-faq).</span></span>

1. <span data-ttu-id="05946-139">[Azure Portal](https://portal.azure.com/) にログオンし、画面左上の **[リソースの作成]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="05946-139">Log on to the [Azure portal](https://portal.azure.com/) and choose **Create a resource** at the top left of the screen.</span></span>

    ![[リソースの作成] の画像](images/create-resource.png)

2. <span data-ttu-id="05946-141">**[モノのインターネット (IoT)]** を選択し、**[Event Hubs]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="05946-141">Select **Internet of Things** and choose **Event Hubs**.</span></span>

    ![[Event Hubs] の画像](images/event-hubs.png)

3. <span data-ttu-id="05946-143">**[名前空間の作成]** で、名前空間の名前を入力します。</span><span class="sxs-lookup"><span data-stu-id="05946-143">In **Create namespace**, enter a namespace name.</span></span> <span data-ttu-id="05946-144">名前空間の名前が使用できることを確認した後、価格レベル (Basic または Standard) を選択します。</span><span class="sxs-lookup"><span data-stu-id="05946-144">After making sure the namespace name is available, choose the pricing tier (Basic or Standard).</span></span> <span data-ttu-id="05946-145">さらに、Azure サブスクリプション、リソース グループ、およびリソースを作成する場所を選択します。</span><span class="sxs-lookup"><span data-stu-id="05946-145">Also, choose an Azure subscription, resource group, and location in which to create the resource.</span></span> <span data-ttu-id="05946-146">**[作成]** を選択して名前空間を作成します。</span><span class="sxs-lookup"><span data-stu-id="05946-146">Choose **Create** to create the namespace.</span></span> <span data-ttu-id="05946-147">システムによるリソースのプロビジョニングが完了するまで、数分かかることがあります。</span><span class="sxs-lookup"><span data-stu-id="05946-147">You might have to wait a few minutes for the system to fully provision the resources.</span></span>

    ![[名前空間の作成] の画像](images/create-namespace.png)

## <a name="step-2-configure-azure-monitor-to-send-security-alerts-from-your-tenant-to-the-event-hub"></a><span data-ttu-id="05946-149">手順 2: テナントからイベント ハブにセキュリティの警告を送信するように Azure Monitor を構成する</span><span class="sxs-lookup"><span data-stu-id="05946-149">Step 2: Configure Azure Monitor to send security alerts from your tenant to the event hub</span></span>

<span data-ttu-id="05946-150">Azure Monitor を使った組織のセキュリティの警告のストリーミングを有効にする操作は、Azure Active Directory (Azure AD) テナント全体で 1 回だけ実行します。</span><span class="sxs-lookup"><span data-stu-id="05946-150">Enabling the streaming of your organization’s security alerts through Azure Monitor is done one time for your entire Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="05946-151">Microsoft Graph セキュリティ API がライセンスされ、有効になっているすべての製品が Azure Monitor にセキュリティ警告を送信し始め、Azure Monitor がコンシューマー アプリケーションにデータをストリーミングし始めます。</span><span class="sxs-lookup"><span data-stu-id="05946-151">All security API licensed and enabled products will begin sending security alerts to Azure Monitor, streaming data to consuming applications.</span></span> <span data-ttu-id="05946-152">組織にライセンスされ、配置された追加の Microsoft Graph セキュリティ API 対応製品は、この同じ Azure Monitor 構成を使用してセキュリティ警告を自動的にストリーミングします。</span><span class="sxs-lookup"><span data-stu-id="05946-152">Any additional security API-enabled products licensed and deployed by your organization will automatically stream security alerts through this same Azure Monitor configuration.</span></span> <span data-ttu-id="05946-153">組織内で追加の統合作業は発生しません。</span><span class="sxs-lookup"><span data-stu-id="05946-153">No further integration work is needed from the organization.</span></span>

<span data-ttu-id="05946-154">セキュリティの警告は、通常は組織内のセキュリティ対応担当者と全体管理者だけが表示できる高い権限を持つデータです。</span><span class="sxs-lookup"><span data-stu-id="05946-154">Security alerts are highly privileged data typically viewable only by security response personnel and global administrators within an organization.</span></span> <span data-ttu-id="05946-155">このため、テナントのセキュリティの警告と SIEM システムの統合を構成する手順では、Azure AD の全体管理者アカウントが必要です。</span><span class="sxs-lookup"><span data-stu-id="05946-155">For this reason, the steps required to configure the integration of a tenant’s security alerts with SIEM systems require an Azure AD Global Administrator account.</span></span> <span data-ttu-id="05946-156">このアカウントは、セットアップ中に組織のセキュリティ警告を Azure Monitor に送信するように要求するときに 1 回だけ使用されます。</span><span class="sxs-lookup"><span data-stu-id="05946-156">This account is only needed one time, during setup, to request your organization’s security alerts be sent to Azure Monitor.</span></span>

> <span data-ttu-id="05946-157">**注:** 現時点では、Azure Monitor の [診断設定] ブレードでテナントレベルのリソースを構成することはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="05946-157">**Note:** At this time, the Azure Monitor Diagnostic settings blade does not allow configuration of tenant-level resources.</span></span> <span data-ttu-id="05946-158">Microsoft Graph セキュリティ API の警告はテナントレベルのリソースです。このリソースでは Azure Resource Manager API を使用して、組織のセキュリティ警告の使用をサポートするように Azure Monitor を構成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="05946-158">Microsoft Graph Security API alerts are a tenant-level resource, which requires using the Azure Resource Manager API to configure Azure Monitor to support consumption of your organization’s security alerts.</span></span>

1. <span data-ttu-id="05946-159">Azure サブスクリプションで "microsoft.insights" (Azure Monitor) をリソース プロバイダーとして登録します。</span><span class="sxs-lookup"><span data-stu-id="05946-159">In your Azure subscription, register "microsoft.insights" (Azure Monitor) as a resource provider.</span></span>  
 > <span data-ttu-id="05946-160">**注:** Azure サブスクリプションで "Microsoft.SecurityGraph" (Microsoft Graph セキュリティ API) をリソース プロバイダーとして登録しないでください。これは、上記で説明したとおり、"Microsoft.SecurityGraph" はテナントレベルのリソースであるためです。</span><span class="sxs-lookup"><span data-stu-id="05946-160">**Note:** Do not register "Microsoft.SecurityGraph" (Microsoft Graph Security API) as a resource provider in your Azure subscription, as “Microsoft.SecurityGraph” is a tenant-level resource as explained above.</span></span> <span data-ttu-id="05946-161">テナントレベルでの構成は後述する手順 6 で行います。</span><span class="sxs-lookup"><span data-stu-id="05946-161">Tenant level configuration will be part of #6 below.</span></span>

2. <span data-ttu-id="05946-162">Azure Resource Manager API を使用して Azure Monitor を構成するには、[ARMClient](https://github.com/projectkudu/ARMClient) ツールを入手します。</span><span class="sxs-lookup"><span data-stu-id="05946-162">To configure Azure Monitor using the Azure Resource Manager API, obtain the [ARMClient](https://github.com/projectkudu/ARMClient) tool.</span></span> <span data-ttu-id="05946-163">このツールは、コマンド ラインから Azure Portal に REST API 呼び出しを送信するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="05946-163">This tool will be used to send REST API calls to the Azure portal from a command line.</span></span>

3. <span data-ttu-id="05946-164">次のような診断設定要求の JSON ファイルを準備します。</span><span class="sxs-lookup"><span data-stu-id="05946-164">Prepare a diagnostic setting request JSON file like the following:</span></span>

<!-- {
  "blockType": "ignored"
} -->

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

  <span data-ttu-id="05946-165">JSON ファイル内の値を次のように置き換えます。</span><span class="sxs-lookup"><span data-stu-id="05946-165">Replace the values in the JSON file as follows:</span></span>

  * <span data-ttu-id="05946-166">**SUBSCRIPTION_ID** は、組織からセキュリティの警告を送信するときに使用するリソース グループとイベント ハブの名前空間をホストする Azure サブスクリプションのサブスクリプション ID です。</span><span class="sxs-lookup"><span data-stu-id="05946-166">**SUBSCRIPTION_ID** is the Subscription ID of the Azure subscription hosting the resource group and event hub namespace where you will be sending security alerts from your organization.</span></span>
  * <span data-ttu-id="05946-167">**RESOURCE_GROUP** は、組織からセキュリティの警告を送信するときに使用するイベント ハブの名前空間を含むリソース グループです。</span><span class="sxs-lookup"><span data-stu-id="05946-167">**RESOURCE_GROUP** is the resource group containing the event hub namespace where you will be sending security alerts from your organization.</span></span>
  * <span data-ttu-id="05946-168">**EVENT_HUB_NAMESPACE** は、組織からセキュリティ警告を送信するときに使用するイベント ハブの名前空間です。</span><span class="sxs-lookup"><span data-stu-id="05946-168">**EVENT_HUB_NAMESPACE** is the event hub namespace where you will be sending security alerts from your organization.</span></span>
  * <span data-ttu-id="05946-169">**“days”:** は、イベント ハブにメッセージを保持する日数です。</span><span class="sxs-lookup"><span data-stu-id="05946-169">**“days”:** 7 is the number of days you want to retain messages in your event hub.</span></span>
  
&nbsp;
4. <span data-ttu-id="05946-170">ARMClient.exe を起動するディレクトリに、このファイルを JSON 形式で保存します。</span><span class="sxs-lookup"><span data-stu-id="05946-170">Save the file as JSON to the directory where you will invoke ARMClient.exe.</span></span> <span data-ttu-id="05946-171">たとえば、ファイル名を **AzMonConfig.json** とします。</span><span class="sxs-lookup"><span data-stu-id="05946-171">For example, name the file **AzMonConfig.json.**</span></span>

5. <span data-ttu-id="05946-172">次のコマンドを実行して ARMClient ツールにサインインします。</span><span class="sxs-lookup"><span data-stu-id="05946-172">Run the following command to sigh in to the ARMClient tool.</span></span> <span data-ttu-id="05946-173">全体管理者アカウントの資格情報を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="05946-173">You will need to be using Global Administrator account credentials.</span></span>

    ``` shell
    ARMClient.exe login
    ```

6. <span data-ttu-id="05946-174">次のコマンドを実行して、セキュリティの警告をイベント ハブの名前空間に送信するように Azure Monitor を構成します。</span><span class="sxs-lookup"><span data-stu-id="05946-174">Run the following command to configure Azure Monitor to send security alerts to your event hub namespace.</span></span> <span data-ttu-id="05946-175">これにより、名前空間の内部にイベント ハブが自動的にプロビジョニングされ、セキュリティの警告のイベント ハブへのフローが開始されます。</span><span class="sxs-lookup"><span data-stu-id="05946-175">This will automatically provision an event hub within the namespace and start the flow of security alerts into the event hub.</span></span> <span data-ttu-id="05946-176">設定名 (この例では **securityApiAlerts**) が JSON ファイルの **name** フィールドに設定した設定名と一致することを確認してください。</span><span class="sxs-lookup"><span data-stu-id="05946-176">Ensure that the setting name (in this example, **securityApiAlerts**) matches the setting name you specified in the JSON file for the **name** field.</span></span>

    ``` shell
    ARMClient.exe put https://management.azure.com/providers/Microsoft.SecurityGraph/diagnosticSettings/securityApiAlerts?api-version=2017-04-01-preview  @".\AzMonConfig.json"
    ```

7. <span data-ttu-id="05946-177">設定が正しく適用されていることを確認するには、次のコマンドを実行して、出力が JSON ファイルの設定と一致していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="05946-177">To verify the settings were applied correctly, run this command and verify that the output matches your JSON file settings.</span></span>

    ``` shell
    ARMClient.exe get https://management.azure.com/providers/Microsoft.SecurityGraph/diagnosticSettings/securityApiAlerts?api-version=2017-04-01-preview
    ```

8. <span data-ttu-id="05946-178">ARMClient ツールを終了します。</span><span class="sxs-lookup"><span data-stu-id="05946-178">Exit the ARMClient tool.</span></span> <span data-ttu-id="05946-179">これで、イベント ハブにテナントのセキュリティの警告を送信するための Azure Monitor の構成が完了しました。</span><span class="sxs-lookup"><span data-stu-id="05946-179">You have now completed the configuration of Azure Monitor to send security alerts from your tenant to event hub.</span></span>

## <a name="step-3-download-and-install-the-azure-monitor-add-on-for-splunk-which-will-allow-splunk-to-consume-security-alerts"></a><span data-ttu-id="05946-180">手順 3: Splunk がセキュリティ警告を使用できるように Splunk 向けの Azure Monitor アドオンをダウンロードしてインストールする</span><span class="sxs-lookup"><span data-stu-id="05946-180">Step 3: Download and install the Azure Monitor Add-on for Splunk which will allow Splunk to consume security alerts</span></span>

1. <span data-ttu-id="05946-181">この統合では [Splunk Enterprise](https://splunkbase.splunk.com/) 展開のみをサポートします。</span><span class="sxs-lookup"><span data-stu-id="05946-181">This integration only supports [Splunk Enterprise](https://splunkbase.splunk.com/) deployments.</span></span>
2. <span data-ttu-id="05946-182">[Splunk 向けの Azure Monitor アドオン](https://github.com/Microsoft/AzureMonitorAddonForSplunk)をダウンロードしてインストールします。</span><span class="sxs-lookup"><span data-stu-id="05946-182">Download and install the [Azure Monitor Add-on for Splunk](https://github.com/Microsoft/AzureMonitorAddonForSplunk).</span></span> <span data-ttu-id="05946-183">インストール手順の詳細については、[インストール](https://github.com/Microsoft/AzureMonitorAddonForSplunk/wiki/Installation)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="05946-183">For detailed installation instructions, see [Installation](https://github.com/Microsoft/AzureMonitorAddonForSplunk/wiki/Installation).</span></span> <span data-ttu-id="05946-184">**バージョン 1.2.9 以降の Splunk 向け Azure Monitor アドオンのみがサポートされています。**</span><span class="sxs-lookup"><span data-stu-id="05946-184">**Only Azure Monitor Add-on for Splunk version 1.2.9 or higher is supported.**</span></span>
3. <span data-ttu-id="05946-185">アドオンを正常にインストールした後、[Azure Monitor アドオン構成 Wiki](https://github.com/Microsoft/AzureMonitorAddonForSplunk/wiki/Configuration-of-Splunk ) で説明されている構成手順に従い、Splunk を構成します。</span><span class="sxs-lookup"><span data-stu-id="05946-185">After successfully installing the Add-on, follow the configuration steps described in the [Azure Monitor add-on configuration wiki](https://github.com/Microsoft/AzureMonitorAddonForSplunk/wiki/Configuration-of-Splunk ) to configure Splunk.</span></span>
4. <span data-ttu-id="05946-186">アドオンのインストール手順に示されているように、アドオンは Splunk Web の [App の管理] ページで有効/無効を切り替えることで動作します。</span><span class="sxs-lookup"><span data-stu-id="05946-186">As indicated in the Add-on installation instructions, the add-on will work by doing a disable/enable cycle on the Manage Apps page in Splunk Web.</span></span> <span data-ttu-id="05946-187">または、Splunk を再起動します。</span><span class="sxs-lookup"><span data-stu-id="05946-187">Or, you can restart Splunk.</span></span>

## <a name="step-4-register-an-application-with-your-tenant-azure-active-directory-which-splunk-will-use-to-read-from-the-event-hub"></a><span data-ttu-id="05946-188">手順 4: Splunk がイベント ハブからの読み取りに使用するアプリケーションをテナントの Azure Active Directory に登録する</span><span class="sxs-lookup"><span data-stu-id="05946-188">Step 4: Register an application with your tenant Azure Active Directory which Splunk will use to read from the event hub</span></span>

<span data-ttu-id="05946-189">Splunk を使用するには、Azure Monitor イベント ハブに対する認証で必要になるアクセス許可とアプリ資格情報が付与されるよう、組織の Azure Active Directory にアプリケーションを登録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="05946-189">Splunk needs an application registration in your organization’s Azure Active Directory to be granted the required permissions and app credentials required to authenticate to the Azure Monitor event hub.</span></span>

1. <span data-ttu-id="05946-190">Azure Portal で、**[アプリの登録]** に移動して **[新しいアプリケーションの登録]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="05946-190">In the Azure portal, go to **App Registrations** and select **New application registration**.</span></span>

    ![[アプリの登録] の画像](images/app-registration.png)

2. <span data-ttu-id="05946-192">アプリケーションの名前を選択し、種類として **[Web アプリ / API]**、サインイン URL として **`https://localhost`** をそれぞれ選択します。</span><span class="sxs-lookup"><span data-stu-id="05946-192">Select a name for your application, choose **Web app / API** for the type, and **`https://localhost`** for the sign-on URL.</span></span> <span data-ttu-id="05946-193">その後、**[作成]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="05946-193">Then select **Create**.</span></span>

    ![Web API の構成](images/app-web-config.png)

3. <span data-ttu-id="05946-195">アプリケーションが作成されたら、**[アプリケーション ID]** を後で Splunk のデータ入力の構成時に使用するためにコピーして保存します。</span><span class="sxs-lookup"><span data-stu-id="05946-195">After the application is created, copy the **Application ID** and save for later use configuring the Splunk data inputs.</span></span> <span data-ttu-id="05946-196">その後、アプリケーション設定に移動して **[キー]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="05946-196">Then go to the application settings and choose **Keys**.</span></span>

    ![Web アプリ ID](images/app-id.png)

    <span data-ttu-id="05946-198">これにより、アプリケーション シークレットと呼ばれる新しいキーを生成できます。</span><span class="sxs-lookup"><span data-stu-id="05946-198">This will allow you to generate a new key, known as an Application Secret.</span></span> <span data-ttu-id="05946-199">キーが生成されたら、**[アプリケーション シークレット]** を後で Splunk のデータ入力の構成時に使用するためにコピーして保存します。</span><span class="sxs-lookup"><span data-stu-id="05946-199">After it's generated, copy the **Application Secret** and save for later use configuring the Splunk data inputs.</span></span>

4. <span data-ttu-id="05946-200">イベント ハブと組織のセキュリティの警告を含む Azure サブスクリプションで、アプリケーションに**閲覧者**のロールを付与します。</span><span class="sxs-lookup"><span data-stu-id="05946-200">Grant the application the role of **Reader** in the Azure subscription containing the event hub with your organization’s security alerts.</span></span>

    ![Azure サブスクリプションの追加](images/add-azure-sub.png)

    <span data-ttu-id="05946-202">サブスクリプションを選択し、**[アクセス制御 (IAM)]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="05946-202">Select your subscription, choose **Access control (IAM)**.</span></span> <span data-ttu-id="05946-203">**[追加]** を選択してアクセス許可を追加します。</span><span class="sxs-lookup"><span data-stu-id="05946-203">Select **Add** to add permissions.</span></span> <span data-ttu-id="05946-204">アプリケーションを選択し、アプリケーションに対して **[閲覧者]** の **[ロール]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="05946-204">Select your application and choose the **Role** of **Reader** for your application.</span></span>

    ![閲覧者のアクセス許可の追加](images/add-reader-perms.png)

    <span data-ttu-id="05946-206">**[保存]** を選択して、アプリケーションに付与したアクセス許可をサブスクリプションに追加します。</span><span class="sxs-lookup"><span data-stu-id="05946-206">Select **Save** to add the permissions granted to your application to the subscription.</span></span>

## <a name="step-5-create-an-azure-key-vault-to-store-the-access-key-for-the-event-hub"></a><span data-ttu-id="05946-207">手順 5: イベント ハブのアクセス キーを格納する Azure Key Vault を作成する</span><span class="sxs-lookup"><span data-stu-id="05946-207">Step 5: Create an Azure Key vault to store the access key for the event hub</span></span>

<span data-ttu-id="05946-208">Azure Key Vault は、アプリケーションが実行時に使用する ID、パスワード、証明書などのシークレットを格納するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="05946-208">Azure key vaults are used to store secrets such as identities, passwords, and certificates for use at runtime by applications.</span></span> <span data-ttu-id="05946-209">この手順では、Splunk が組織のセキュリティの警告を含む Azure イベント ハブに接続してセキュリティの警告を読み取るのに必要なシークレットを格納する Azure Key Vault を作成します。</span><span class="sxs-lookup"><span data-stu-id="05946-209">In this step you will create an Azure key vault to store the secrets needed for Splunk to connect and read from the Azure event hubs containing your organization’s security alerts.</span></span>

1. <span data-ttu-id="05946-210">Azure Portal で、**[キー コンテナー]** に移動して **[追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="05946-210">In the Azure portal, go to **Key vaults** and select **Add**.</span></span>

    ![キー コンテナーの追加](images/add-key-vaults.png)

2. <span data-ttu-id="05946-212">新しいキー コンテナーの作成時に、**[アクセス ポリシー]** を選択して、手順 4 で登録したアプリケーション用の新しいアクセス ポリシーを追加します。</span><span class="sxs-lookup"><span data-stu-id="05946-212">When creating the new key vault, select **Access policies** to add a new access policy for the application you just registered in Step 4.</span></span> <span data-ttu-id="05946-213">シークレットの **[取得]** アクセス許可をアプリケーションに付与します。</span><span class="sxs-lookup"><span data-stu-id="05946-213">Grant the **Get** secret permissions to your application.</span></span> <span data-ttu-id="05946-214">これで、Splunk が登録済みのアプリケーションとして動作し、この Azure Key Vault に格納されているキー (シークレット) にアクセスできるようになります。</span><span class="sxs-lookup"><span data-stu-id="05946-214">This will allow Splunk, acting as the registered application, to access the keys (secrets) stored in this Azure key vault.</span></span>

    ![アクセス ポリシーの追加](images/add-access-policies.png)

    <span data-ttu-id="05946-216">**[作成]** を選択して、新しい Azure Key Vault の作成を完了します。</span><span class="sxs-lookup"><span data-stu-id="05946-216">Select **Create** to complete the creation of your new Azure key vault.</span></span>

3. <span data-ttu-id="05946-217">キー コンテナー内に新しいシークレットを生成して、イベント ハブの名前空間へのアクセス キーを格納します。</span><span class="sxs-lookup"><span data-stu-id="05946-217">Generate a new secret in your key vault to store the access key to your event hub namespace.</span></span> <span data-ttu-id="05946-218">最初に、イベント ハブの名前空間を開き、**[共有アクセス ポリシー]** を選択して、イベント ハブの名前空間へのアクセス キーを取得します。</span><span class="sxs-lookup"><span data-stu-id="05946-218">First, grab the access key to your event hub namespace by opening your event hub namespace and selecting **Shared access policies**.</span></span> <span data-ttu-id="05946-219">リストから **RootManageSharedAccessKey** ポリシーを選択し、リストから**主キー**をコピーします。</span><span class="sxs-lookup"><span data-stu-id="05946-219">Select the **RootManageSharedAccessKey** policy from the list and copy the **Primary Key** from the list.</span></span>

    ![共有アクセス ポリシーの取得](images/get-shared-policies.png)

4. <span data-ttu-id="05946-221">キー コンテナーを開き、**[シークレット]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="05946-221">Open your key vault and select **Secrets**.</span></span> <span data-ttu-id="05946-222">**[生成/インポート]** を選択して、キー コンテナーに新しいシークレットを追加します。</span><span class="sxs-lookup"><span data-stu-id="05946-222">Choose **Generate/Import** to add a new secret to the key vault.</span></span> <span data-ttu-id="05946-223">イベント ハブの名前空間 **RootManageSharedAccessKey** の**主キー**を貼り付けます。</span><span class="sxs-lookup"><span data-stu-id="05946-223">Paste in the **Primary key** from the event hub namespace **RootManageSharedAccessKey**.</span></span>

    ![新しいシークレットの生成](images/generate-new-secret.png)

5. <span data-ttu-id="05946-225">シークレットが作成されたら、シークレットを選択して **[シークレットのバージョン]** をコピーします。</span><span class="sxs-lookup"><span data-stu-id="05946-225">After it's created, select the secret and copy the **Secret Version** of the secret.</span></span> <span data-ttu-id="05946-226">これは、手順 6 で Splunk のデータ入力を構成するときに使用されます。</span><span class="sxs-lookup"><span data-stu-id="05946-226">This will be used later in Step 6 to configure Splunk data inputs.</span></span>

    ![シークレットのバージョン](images/secret-version.png)

## <a name="step-6-configure-the-splunk-data-inputs-to-consume-security-alerts-stored-in-the-event-hub"></a><span data-ttu-id="05946-228">手順 6: イベント ハブに格納されているセキュリティの警告を使用するように Splunk のデータ入力を構成する</span><span class="sxs-lookup"><span data-stu-id="05946-228">Step 6: Configure the Splunk data inputs to consume security alerts stored in the event hub</span></span>

<span data-ttu-id="05946-229">セットアップ プロセスを完了する最後の手順では、前の手順で作成したイベント ハブ、アプリケーション、およびシークレットを利用するように Splunk のデータ入力を構成します。</span><span class="sxs-lookup"><span data-stu-id="05946-229">The last step to complete the setup process is to configure Splunk data inputs to utilize the event hub, application, and secrets you created in previous steps.</span></span>

1. <span data-ttu-id="05946-230">[Splunk の構成](https://github.com/Microsoft/AzureMonitorAddonForSplunk/wiki/Configuration-of-Splunk)の説明に従って Splunk のデータ入力を開き、Azure Monitor アドオン用に構成します。</span><span class="sxs-lookup"><span data-stu-id="05946-230">Follow the instructions in the [Configuration of Splunk](https://github.com/Microsoft/AzureMonitorAddonForSplunk/wiki/Configuration-of-Splunk) topic to open and configure Splunk data inputs for the Azure Monitor Add-on.</span></span> <span data-ttu-id="05946-231">**[設定]** および **[データ入力]** に移動します。</span><span class="sxs-lookup"><span data-stu-id="05946-231">Go to **Settings** and **Data Inputs**.</span></span> <span data-ttu-id="05946-232">**[Azure Monitor 診断ログ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="05946-232">Choose **Azure Monitor Diagnostic Logs**.</span></span>
2. <span data-ttu-id="05946-233">**[新規]** を選択し、前の手順で取得した値を使用してすべての必須フィールドに入力します。</span><span class="sxs-lookup"><span data-stu-id="05946-233">Select **New** and input all the required fields using the values obtained in the previous steps.</span></span> <span data-ttu-id="05946-234">次の図では、すべての必須フィールドにこの記事で使用した例の値が入力されています。</span><span class="sxs-lookup"><span data-stu-id="05946-234">The following image shows all the required fields using the values from the previous examples in this article.</span></span>

    ![Azure Monitor のフィールド](images/azure-monitor-fields.png)

3. <span data-ttu-id="05946-236">**[次へ]** を選択すると、Azure Monitor から取り込まれた組織のセキュリティ警告の検索が開始されます。</span><span class="sxs-lookup"><span data-stu-id="05946-236">Select **Next** and begin searching your organization’s security alerts ingested from Azure Monitor.</span></span>

## <a name="optional-use-splunk-search-to-explore-data"></a><span data-ttu-id="05946-237">(省略可能) Splunk 検索機能を使用してデータを探索します。</span><span class="sxs-lookup"><span data-stu-id="05946-237">(Optional) Use Splunk Search to explore data</span></span>

<span data-ttu-id="05946-238">Azure Monitor Splunk プラグインのセットアップが完了すると、Splunk インスタンスが構成済みのイベント ハブからイベントを取得するようになります。</span><span class="sxs-lookup"><span data-stu-id="05946-238">After you have set up the Azure Monitor Splunk plugin, your Splunk instance will start retrieving events from the configured event hub.</span></span> <span data-ttu-id="05946-239">既定では、Splunk は Microsoft Graph セキュリティ API の警告スキーマの各プロパティにインデックスを付けて検索可能にします。</span><span class="sxs-lookup"><span data-stu-id="05946-239">By default, Splunk will index each property of the Microsoft Graph Security API alert schema to allow searching.</span></span>

<span data-ttu-id="05946-240">Microsoft Graph セキュリティ API の警告を検索する場合、ダッシュボードを作成する場合、または検索クエリで Splunk の警告を設定する場合は、Splunk で [apps] -> [Search & Reporting app] に移動します。</span><span class="sxs-lookup"><span data-stu-id="05946-240">To search for Microsoft Graph Security API alerts, to create dashboards, or to set Splunk alerts with your search query, navigate to apps -> Search & Reporting app in Splunk.</span></span>

<span data-ttu-id="05946-241">**例**:</span><span class="sxs-lookup"><span data-stu-id="05946-241">Examples</span></span><br/>
<span data-ttu-id="05946-242">Graph セキュリティ警告を検索する場合:</span><span class="sxs-lookup"><span data-stu-id="05946-242">Try searching Graph Security alerts:</span></span>

- <span data-ttu-id="05946-243">Microsoft Graph セキュリティ API によって検出されたすべての警告を取得するために、検索バーに `sourcetype="amdl:securitygraph:alert"` と入力します。</span><span class="sxs-lookup"><span data-stu-id="05946-243">Type `sourcetype="amdl:securitygraph:alert"` in the search bar to get all alerts surfaced through the Microsoft Graph Security API.</span></span> <span data-ttu-id="05946-244">右側に、Azure Monitor ログのトップレベル プロパティが表示されます。このログのプロパティ フィールドに、Graph セキュリティ警告が一覧されます。</span><span class="sxs-lookup"><span data-stu-id="05946-244">On the right-hand side, you will see the top-level properties of Azure Monitor log where Graph Security alert is under properties field.</span></span><br/>
- <span data-ttu-id="05946-245">左側のウィンドウには、選択されたフィールドと興味深いフィールドが表示されます。</span><span class="sxs-lookup"><span data-stu-id="05946-245">On the left pane, you will see selected fields and interesting fields.</span></span> <span data-ttu-id="05946-246">選択されたフィールドを使用して、ダッシュボードや Splunk の警告を作成できます。また、選択されたフィールドを右クリックして、フィールドを追加または削除することもできます。</span><span class="sxs-lookup"><span data-stu-id="05946-246">You can use selected fields to create dashboards or Splunk alerts, you can also add or remove selected fields by right-clicking on the fields.</span></span>  
> <span data-ttu-id="05946-247">**注:** 以下の検索クエリに示されているように、必要に応じて検索を絞り込むことができます。</span><span class="sxs-lookup"><span data-stu-id="05946-247">**Note:** As shown in the following search query, you can restrict your search as needed.</span></span> <span data-ttu-id="05946-248">この例では、Graph セキュリティ警告を、Azure Security Center からの重要度高の警告に絞り込んでいます。</span><span class="sxs-lookup"><span data-stu-id="05946-248">In the example, we filter the Graph Security Alerts by high severity alerts from Azure Security Center.</span></span> <span data-ttu-id="05946-249">また、表示対象の選択されたフィールドとして `eventDatetime`、`severity`、`status`、`provider` を使用しています。</span><span class="sxs-lookup"><span data-stu-id="05946-249">We also used `eventDatetime`, `severity`, `status`, and `provider` as selected fields to be displayed.</span></span> <span data-ttu-id="05946-250">高度な検索条件については、[Splunk 検索チュートリアル](https://docs.splunk.com/Documentation/Splunk/7.1.2/SearchTutorial/WelcometotheSearchTutorial)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="05946-250">For more advance search terms, see [Splunk search tutorials](https://docs.splunk.com/Documentation/Splunk/7.1.2/SearchTutorial/WelcometotheSearchTutorial).</span></span>

 ![splunk_search_query](images/splunk-search-query.png)
> <span data-ttu-id="05946-252">検索クエリ: `sourcetype="amdl:securitygraph:alert" "properties.vendorInformation.provider"=ASC "properties.severity"=High | rename properties.eventDataTime as eventDateTime properties.severity as severity properties.vendorInformation.provider as provider properties.status as status`</span><span class="sxs-lookup"><span data-stu-id="05946-252">search query`sourcetype="amdl:securitygraph:alert" "properties.vendorInformation.provider"=ASC "properties.severity"=High | rename properties.eventDataTime as eventDateTime properties.severity as severity properties.vendorInformation.provider as provider properties.status as status`</span></span>

<span data-ttu-id="05946-253">Splunk では、画面右上にある [名前を付けて保存] メニュー オプションを使用して、検索結果に対して複数の操作を行うこともできます。</span><span class="sxs-lookup"><span data-stu-id="05946-253">Splunk also allows multiple actions on search results using the "Save As" menu option in top right of the screen.</span></span> <span data-ttu-id="05946-254">検索フィルターに基づくレポート、ダッシュボード、パネル、または警告を作成できます。</span><span class="sxs-lookup"><span data-stu-id="05946-254">You can create Reports, Dashboard Panels, or Alerts based on your search filter.</span></span>
<span data-ttu-id="05946-255">以下に示すダッシュボードの例では、前のクエリに基づくイベント ストリームを表示しています。各イベントのドリルダウン リンクを追加することで、Microsoft Graph サイト上で詳細情報にアクセスできるようになります。</span><span class="sxs-lookup"><span data-stu-id="05946-255">Below is an example of a dashboard with an event stream based on the previous query: You can add a drilldown link to each event to further access the details on Microsoft Graph site.</span></span> <span data-ttu-id="05946-256">[Splunk のドリルダウンに関するドキュメント](https://docs.splunk.com/Documentation/Splunk/7.1.2/Viz/DrilldownIntro)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="05946-256">See [Splunk drilldown documentation](https://docs.splunk.com/Documentation/Splunk/7.1.2/Viz/DrilldownIntro).</span></span>

 ![splunk_search_results](images/splunk-search-results.png)

<span data-ttu-id="05946-258">または、タイムライン グラフとしてダッシュボードを作成することもできます。</span><span class="sxs-lookup"><span data-stu-id="05946-258">Or you can create a dashboard as a timeline chart:</span></span>

 ![splunk_search_timeline](images/splunk-search-timeline.png)

<span data-ttu-id="05946-260">詳しくは、[Splunk の検索とレポートに関するチュートリアル](https://docs.splunk.com/Documentation/Splunk/7.1.2/SearchTutorial/WelcometotheSearchTutorial)に従ってください。</span><span class="sxs-lookup"><span data-stu-id="05946-260">You can follow [Splunk Search & Report tutorial](https://docs.splunk.com/Documentation/Splunk/7.1.2/SearchTutorial/WelcometotheSearchTutorial) for more details.</span></span>

