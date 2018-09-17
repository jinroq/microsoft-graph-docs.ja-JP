# <a name="auditactor-resource-type"></a><span data-ttu-id="b06aa-101">auditActor リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b06aa-101">auditActor resource type</span></span>

> <span data-ttu-id="b06aa-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b06aa-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b06aa-103">監査アクターのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="b06aa-103">A class containing the properties for Audit Actor.</span></span>
## <a name="properties"></a><span data-ttu-id="b06aa-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b06aa-104">Properties</span></span>
|<span data-ttu-id="b06aa-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b06aa-105">Property</span></span>|<span data-ttu-id="b06aa-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="b06aa-106">Type</span></span>|<span data-ttu-id="b06aa-107">説明</span><span class="sxs-lookup"><span data-stu-id="b06aa-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b06aa-108">型</span><span class="sxs-lookup"><span data-stu-id="b06aa-108">type</span></span>|<span data-ttu-id="b06aa-109">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b06aa-109">String</span></span>|<span data-ttu-id="b06aa-110">アクターの種類。</span><span class="sxs-lookup"><span data-stu-id="b06aa-110">Actor Type.</span></span>|
|<span data-ttu-id="b06aa-111">userPermissions</span><span class="sxs-lookup"><span data-stu-id="b06aa-111">userPermissions</span></span>|<span data-ttu-id="b06aa-112">String コレクション</span><span class="sxs-lookup"><span data-stu-id="b06aa-112">String collection</span></span>|<span data-ttu-id="b06aa-113">監査の実行時におけるユーザーのアクセス許可の一覧。</span><span class="sxs-lookup"><span data-stu-id="b06aa-113">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="b06aa-114">applicationId</span><span class="sxs-lookup"><span data-stu-id="b06aa-114">applicationId</span></span>|<span data-ttu-id="b06aa-115">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b06aa-115">String</span></span>|<span data-ttu-id="b06aa-116">AAD アプリケーション ID。</span><span class="sxs-lookup"><span data-stu-id="b06aa-116">AAD Application Id.</span></span>|
|<span data-ttu-id="b06aa-117">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="b06aa-117">applicationDisplayName</span></span>|<span data-ttu-id="b06aa-118">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b06aa-118">String</span></span>|<span data-ttu-id="b06aa-119">アプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="b06aa-119">Name of the Application.</span></span>|
|<span data-ttu-id="b06aa-120">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b06aa-120">userPrincipalName</span></span>|<span data-ttu-id="b06aa-121">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b06aa-121">String</span></span>|<span data-ttu-id="b06aa-122">ユーザー プリンシパル名 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="b06aa-122">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="b06aa-123">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="b06aa-123">servicePrincipalName</span></span>|<span data-ttu-id="b06aa-124">文字列</span><span class="sxs-lookup"><span data-stu-id="b06aa-124">String</span></span>|<span data-ttu-id="b06aa-125">サービス プリンシパル名 (SPN)。</span><span class="sxs-lookup"><span data-stu-id="b06aa-125">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="b06aa-126">ipAddress</span><span class="sxs-lookup"><span data-stu-id="b06aa-126">ipAddress</span></span>|<span data-ttu-id="b06aa-127">文字列</span><span class="sxs-lookup"><span data-stu-id="b06aa-127">String</span></span>|<span data-ttu-id="b06aa-128">IPAddress。</span><span class="sxs-lookup"><span data-stu-id="b06aa-128">IPAddress.</span></span>|
|<span data-ttu-id="b06aa-129">userId</span><span class="sxs-lookup"><span data-stu-id="b06aa-129">userId</span></span>|<span data-ttu-id="b06aa-130">文字列</span><span class="sxs-lookup"><span data-stu-id="b06aa-130">String</span></span>|<span data-ttu-id="b06aa-131">ユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="b06aa-131">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b06aa-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b06aa-132">Relationships</span></span>
<span data-ttu-id="b06aa-133">なし</span><span class="sxs-lookup"><span data-stu-id="b06aa-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b06aa-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b06aa-134">JSON Representation</span></span>
<span data-ttu-id="b06aa-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b06aa-135">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditActor"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.auditActor",
  "type": "String",
  "userPermissions": [
    "String"
  ],
  "applicationId": "String",
  "applicationDisplayName": "String",
  "userPrincipalName": "String",
  "servicePrincipalName": "String",
  "ipAddress": "String",
  "userId": "String"
}
```








