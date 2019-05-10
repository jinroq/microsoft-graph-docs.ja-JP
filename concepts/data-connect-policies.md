---
title: Microsoft Graph データ接続のポリシーとライセンス
description: サポートされているポリシー、および ISV アクセス SKU を組織に割り当てる方法を説明します。
author: tlenig
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: 2f96f099289346455a31ea42c4cb643eb997d558
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629916"
---
# <a name="microsoft-graph-data-connect-policies-and-licensing"></a><span data-ttu-id="7ab03-103">Microsoft Graph データ接続のポリシーとライセンス</span><span class="sxs-lookup"><span data-stu-id="7ab03-103">Microsoft Graph data connect policies and licensing</span></span>

<span data-ttu-id="7ab03-104">Microsoft Graph データ接続は、[Azure マネージド アプリケーション](https://docs.microsoft.com/ja-JP/azure/managed-applications/overview)を使用して、ユーザーがソリューションを作成し、顧客の Azure 環境にそのソリューションをデプロイできるようにしています。</span><span class="sxs-lookup"><span data-stu-id="7ab03-104">Microsoft Graph data connect uses [Azure managed applications](https://docs.microsoft.com/ja-JP/azure/managed-applications/overview) to allow you to create and deploy your solutions in your customer's Azure environment.</span></span> <span data-ttu-id="7ab03-105">マネージド アプリケーションを使用すると、特定の Azure ポリシーをサポートできるため、ユーザーが作成したアプリケーションを使用する顧客に対して、一層の信頼性と快適性を提供できます。</span><span class="sxs-lookup"><span data-stu-id="7ab03-105">Managed applications allow you to support certain Azure policies, giving customers greater confidence and comfortability when using your applications.</span></span> <span data-ttu-id="7ab03-106">さらに、データ接続を介してアプリケーションがデータにアクセスできるようにするには、ユーザーが Microsoft からライセンスを購入し、ユーザー自身の組織またはユーザーのアプリケーションをインストールする組織にライセンスを適用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7ab03-106">Additionally, you must purchase and apply licenses from Microsoft your organization or the organizations that install your applications, in order to allow the application to access data through data connect.</span></span>

## <a name="policies"></a><span data-ttu-id="7ab03-107">ポリシー</span><span class="sxs-lookup"><span data-stu-id="7ab03-107">Policies</span></span>

<span data-ttu-id="7ab03-108">Office 365 のデータを使用して構築された Azure マネージド アプリケーションでは、次の Azure ポリシーがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="7ab03-108">The following Azure policies are supported for an Azure managed application built using Office 365 data:</span></span>

- [<span data-ttu-id="7ab03-109">ADLS Gen1 暗号化必須ポリシー</span><span class="sxs-lookup"><span data-stu-id="7ab03-109">ADLS Gen1 Encryption Required Policy</span></span>](https://docs.microsoft.com/ja-JP/azure/azure-policy/scripts/enforce-datalakestore-encryption)

<span data-ttu-id="7ab03-110">Azure Marketplace の発行時にポリシーのいずれかを選択する場合、そのポリシーのコンプライアンスの状態が確認され、アプリケーションのすべてのインストールに対して適用されます。</span><span class="sxs-lookup"><span data-stu-id="7ab03-110">When you select any of the policies during Azure marketplace publishing, the policy compliance status will be checked and enforced for all installations of your application.</span></span> <span data-ttu-id="7ab03-111">選択され、準拠していることが確認されたポリシーすべては、データ要求の一部として、データの承認者に表示されます。</span><span class="sxs-lookup"><span data-stu-id="7ab03-111">All selected policies that are compliant will be shown to the data approvers as part of the data request.</span></span> <span data-ttu-id="7ab03-112">ポリシーのコンプライアンス違反は、パイプラインの実行が失敗し、データ抽出が停止する原因となります。</span><span class="sxs-lookup"><span data-stu-id="7ab03-112">Any policy compliance violation would cause the pipeline run to fail and stop the data extraction.</span></span>

<span data-ttu-id="7ab03-113">その他のポリシーに関してサポートをご希望の場合は、[UserVoice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests?category_id=359581) からお知らせください。</span><span class="sxs-lookup"><span data-stu-id="7ab03-113">If you would like to request support for additional policies , let us know on [UserVoice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests?category_id=359581).</span></span>

## <a name="licensing"></a><span data-ttu-id="7ab03-114">ライセンス</span><span class="sxs-lookup"><span data-stu-id="7ab03-114">Licensing</span></span>

<span data-ttu-id="7ab03-115">Microsoft Graph データ接続ツールセットには、Workplace Analytics からアクセスできます。これは、ユーザーごとに 1 か月単位でライセンスされます。</span><span class="sxs-lookup"><span data-stu-id="7ab03-115">Access to the Microsoft Graph data connect toolset is available through Workplace Analytics, which is licensed on a per-user, per-month basis.</span></span>  <span data-ttu-id="7ab03-116">Workplace Analytics を使用する組織は、社内または独立系ソフトウェア ベンダー (ISV) によって開発されたアプリケーションに組織の大規模なデータへのアクセスを付与し管理することによって、Office 365 のデータからさらに多くの分析情報を得ることができます。</span><span class="sxs-lookup"><span data-stu-id="7ab03-116">Organizations with Workplace Analytics can extend their insights from Office 365 data by granting and governing access to their data at scale to applications developed in-house or by independent software vendors (ISVs).</span></span> <span data-ttu-id="7ab03-117">購入方法を含む詳細については、[Workplace Analytics 製品ページ](https://products.office.com/ja-JP/business/workplace-analytics)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="7ab03-117">To learn more, including how to purchase, visit the [Workplace Analytics product page](https://products.office.com/ja-JP/business/workplace-analytics).</span></span>

<span data-ttu-id="7ab03-118">ISV を対象として、Workplace Analytics を購入していない顧客向けにアプリケーションを構築するためのオプションも用意されています。</span><span class="sxs-lookup"><span data-stu-id="7ab03-118">If you’re an ISV, we also provide an option for you to build applications for customers who have not purchased Workplace Analytics.</span></span> <span data-ttu-id="7ab03-119">これには、そのアプリケーションが Microsoft Graph データ接続を介してアクセスするすべてのユーザーに関連付けるのに十分なライセンスを、そのアプリケーションを購入する顧客ごとに ISV が購入する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7ab03-119">To do so, you must purchase enough licenses to associate them with all the users your application will access through Microsoft Graph data connect, for each customer who purchases your application.</span></span> <span data-ttu-id="7ab03-120">このオプションは、Workplace Analytics のライセンスと併用できます。</span><span class="sxs-lookup"><span data-stu-id="7ab03-120">You can use this option along with Workplace Analytics licenses.</span></span> <span data-ttu-id="7ab03-121">ISV は、Microsoft Graph データ接続のライセンスのインスタンスを、顧客による各インストールと関連付けるための手順を実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7ab03-121">You’ll need to take steps to associate instances of the Microsoft Graph data connect license with each of their customer installations.</span></span>

### <a name="isvs-using-the-microsoft-graph-data-connect-license"></a><span data-ttu-id="7ab03-122">Microsoft Graph データ接続のライセンスを使用する ISV</span><span class="sxs-lookup"><span data-stu-id="7ab03-122">ISVs using the Microsoft Graph data connect license</span></span>
<span data-ttu-id="7ab03-123">データ接続のライセンスを使用する ISV は、ライセンスの割り当てを保存および処理するために [Azure Key Vault](https://azure.microsoft.com/ja-JP/services/key-vault/) を利用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7ab03-123">If you're an ISV using the data connect license, you must utilized [Azure Key Vault](https://azure.microsoft.com/ja-JP/services/key-vault/) to store and process the license assignment.</span></span> <span data-ttu-id="7ab03-124">したがって、[Key Vault を作成する](https://docs.microsoft.com/ja-JP/azure/key-vault/quick-create-portal)ことが必要になります。</span><span class="sxs-lookup"><span data-stu-id="7ab03-124">You will need to [create a Key Vault](https://docs.microsoft.com/ja-JP/azure/key-vault/quick-create-portal).</span></span> <span data-ttu-id="7ab03-125">作成中、Key Vault の URI 値をメモしてください。</span><span class="sxs-lookup"><span data-stu-id="7ab03-125">During creation, note the Key Vault URI value.</span></span> <span data-ttu-id="7ab03-126">この値は、Key Vault を参照するアプリケーション定義で使用されます。</span><span class="sxs-lookup"><span data-stu-id="7ab03-126">It will be used in the application definition to reference the Key Vault.</span></span> <span data-ttu-id="7ab03-127">Key Vault を作成したら、アプリケーションの ARM テンプレートの Source Linked Service で使用される SPN が Key Vault にアクセスできていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="7ab03-127">After you create the Key Vault, ensure that the SPN used in the Source Linked Service of the application's ARM template has access to it.</span></span> <span data-ttu-id="7ab03-128">これを行うには、Key Vault インスタンスの **[アクセス ポリシー]** ウィンドウに移動し、SPN によって参照されるアプリケーション用のアクセス ポリシーを作成して、そのアプリケーションに **Get** と **List** のアクセス許可を割り当てます。</span><span class="sxs-lookup"><span data-stu-id="7ab03-128">To do so, go to the **Access Policies** pane of the Key Vault instance, create an access policy for the application referenced by the SPN, and assign **Get** and **List** permissions to the application.</span></span> 

![Key Vault へのアクセス ポリシーを作成する](images/data-connect-keyvault-access.png)

<span data-ttu-id="7ab03-130">Microsoft Graph データ接続の組織へのライセンスの割り当ては、Key Vault ではシークレットとして提供されます。</span><span class="sxs-lookup"><span data-stu-id="7ab03-130">The assignment of Microsoft Graph data connect licenses to organizations is provided as a secret in the Key Vault.</span></span> <span data-ttu-id="7ab03-131">これを行うには、以下のようにします。</span><span class="sxs-lookup"><span data-stu-id="7ab03-131">To do so:</span></span>
1. <span data-ttu-id="7ab03-132">Key Vault に移動し、**[生成/インポート]** で手動シークレットを作成します。</span><span class="sxs-lookup"><span data-stu-id="7ab03-132">Go to the Key Vault and under **Generate/Import**, create a manual secret.</span></span> <span data-ttu-id="7ab03-133">シークレットの名前は **MGdcSKUMapping** とする必要があります。また、シークレットの値には、テナントの ID とそのテナントに割り当てられているライセンス数を次の形式で含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="7ab03-133">The name of the secret must be **MGdcSKUMapping** and the value of the secret must contain the ID of the tenant and the number of licenses allocated to that tenant, in the following format.</span></span>

`{"tenantId1" : 20, "tenantId2" : 35, "tenantId3" : 12}`

2. <span data-ttu-id="7ab03-134">値を設定したら、有効になっていることを確認し、**[作成]** を選択して、デプロイを開始します。</span><span class="sxs-lookup"><span data-stu-id="7ab03-134">After setting the value, make sure that it is enabled and select **Create** to begin the deployment.</span></span> 

![Key Vault にシークレットを作成する](images/data-connect-keyvault-create.png)

3. <span data-ttu-id="7ab03-136">また、作成した Key Vault を参照するアプリケーションの ARM テンプレートを更新する必要もあります。</span><span class="sxs-lookup"><span data-stu-id="7ab03-136">You also need to update the application's ARM template to reference the Key Vault that you created.</span></span> <span data-ttu-id="7ab03-137">これには、**LicenseKeyVaultUri** プロパティに、Key Vault の作成時にメモした **KeyVaultUri** 値を入力します。</span><span class="sxs-lookup"><span data-stu-id="7ab03-137">To do so, populated the **LicenseKeyVaultUri** property, which must be populated with the **KeyVaultUri** value you noted during creation.</span></span> <span data-ttu-id="7ab03-138">このプロパティは、次に示すように、アプリケーションの ARM テンプレートの Source Linked Service で提供されます。</span><span class="sxs-lookup"><span data-stu-id="7ab03-138">This property is provided in the Source Linked Service of the application's ARM template, as shown.</span></span> 

```
"properties": {
        "type": "Office365",
            "description": "Source O365 linked service",
            "typeProperties": {
                   "office365tenantId": "[subscription().tenantId]",
        "PrivacyPolicyUri": "http://www.wkw.com/privacy",
        "TermsOfUseUri": "http://www.wkw.com/tos",
        "servicePrincipalId": "[variables('sourceLinkedServicePrincipalId')]",
        "servicePrincipalKey": {
                           "type": "SecureString",
                "value": "[variables('sourceLinkedServicePrincipalKey')]"
        },
        "servicePrincipalTenantId": "[variables('sourceLinkedServicePrincipalTenantId')]",
        "LicenseKeyVaultUri": "<KeyVaultUri>",
            }
    }
```

<span data-ttu-id="7ab03-139">データ接続は、各パイプラインを実行する前に、Key Vault のシークレットを参照します。</span><span class="sxs-lookup"><span data-stu-id="7ab03-139">Data connect will reference the secret in the Key Vault before each pipeline run.</span></span> <span data-ttu-id="7ab03-140">各ユーザーにデータを提供するのに十分なライセンスが組織に割り当てられていない場合、または Key Vault にアクセスできない場合、パイプラインは失敗します。</span><span class="sxs-lookup"><span data-stu-id="7ab03-140">It will fail the pipeline if there aren't enough licenses assigned to the organization to provide data for each user, or if the Key Vault is inaccessible.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="7ab03-141">次のステップ</span><span class="sxs-lookup"><span data-stu-id="7ab03-141">Next Steps</span></span>
<span data-ttu-id="7ab03-142">その他のポリシーに関してサポートをご希望の場合は、[UserVoice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests?category_id=359581) からお知らせください。</span><span class="sxs-lookup"><span data-stu-id="7ab03-142">If you would like to request support for additional policies, let us know on [UserVoice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests?category_id=359581).</span></span> <span data-ttu-id="7ab03-143">購入方法を含む Workplace Analytics の詳細については、[Workplace Analytics 製品ページ](https://products.office.com/ja-JP/business/workplace-analytics)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="7ab03-143">To learn more about Workplace Analytics, including how to purchase, visit the [Workplace Analytics product page](https://products.office.com/ja-JP/business/workplace-analytics).</span></span>
