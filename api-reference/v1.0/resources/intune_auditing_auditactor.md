# <a name="auditactor-resource-type"></a><span data-ttu-id="2c008-101">auditActor リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2c008-101">auditActor resource type</span></span>

> <span data-ttu-id="2c008-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2c008-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2c008-103">監査アクターのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="2c008-103">A class containing the properties for Audit Actor.</span></span>
## <a name="properties"></a><span data-ttu-id="2c008-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2c008-104">Properties</span></span>
|<span data-ttu-id="2c008-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2c008-105">Property</span></span>|<span data-ttu-id="2c008-106">型</span><span class="sxs-lookup"><span data-stu-id="2c008-106">Type</span></span>|<span data-ttu-id="2c008-107">説明</span><span class="sxs-lookup"><span data-stu-id="2c008-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c008-108">type</span><span class="sxs-lookup"><span data-stu-id="2c008-108">type</span></span>|<span data-ttu-id="2c008-109">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="2c008-109">String</span></span>|<span data-ttu-id="2c008-110">アクターの種類。</span><span class="sxs-lookup"><span data-stu-id="2c008-110">Actor Type.</span></span>|
|<span data-ttu-id="2c008-111">permissions</span><span class="sxs-lookup"><span data-stu-id="2c008-111">permissions</span></span>|<span data-ttu-id="2c008-112">String コレクション</span><span class="sxs-lookup"><span data-stu-id="2c008-112">String collection</span></span>|<span data-ttu-id="2c008-113">監査の実行時におけるユーザーのアクセス許可の一覧。</span><span class="sxs-lookup"><span data-stu-id="2c008-113">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="2c008-114">userPermissions</span><span class="sxs-lookup"><span data-stu-id="2c008-114">userPermissions</span></span>|<span data-ttu-id="2c008-115">String コレクション</span><span class="sxs-lookup"><span data-stu-id="2c008-115">String collection</span></span>|<span data-ttu-id="2c008-116">監査の実行時におけるユーザーのアクセス許可の一覧。</span><span class="sxs-lookup"><span data-stu-id="2c008-116">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="2c008-117">applicationId</span><span class="sxs-lookup"><span data-stu-id="2c008-117">applicationId</span></span>|<span data-ttu-id="2c008-118">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="2c008-118">String</span></span>|<span data-ttu-id="2c008-119">AAD アプリケーション ID。</span><span class="sxs-lookup"><span data-stu-id="2c008-119">AAD Application Id.</span></span>|
|<span data-ttu-id="2c008-120">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="2c008-120">applicationDisplayName</span></span>|<span data-ttu-id="2c008-121">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="2c008-121">String</span></span>|<span data-ttu-id="2c008-122">アプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="2c008-122">Name of the Application.</span></span>|
|<span data-ttu-id="2c008-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2c008-123">userPrincipalName</span></span>|<span data-ttu-id="2c008-124">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="2c008-124">String</span></span>|<span data-ttu-id="2c008-125">ユーザー プリンシパル名 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="2c008-125">User principal name (UPN)</span></span>|
|<span data-ttu-id="2c008-126">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="2c008-126">servicePrincipalName</span></span>|<span data-ttu-id="2c008-127">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="2c008-127">String</span></span>|<span data-ttu-id="2c008-128">サービス プリンシパル名 (SPN)。</span><span class="sxs-lookup"><span data-stu-id="2c008-128">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="2c008-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="2c008-129">ipAddress</span></span>|<span data-ttu-id="2c008-130">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="2c008-130">String</span></span>|<span data-ttu-id="2c008-131">IPAddress。</span><span class="sxs-lookup"><span data-stu-id="2c008-131">IPAddress.</span></span>|
|<span data-ttu-id="2c008-132">userId</span><span class="sxs-lookup"><span data-stu-id="2c008-132">userId</span></span>|<span data-ttu-id="2c008-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="2c008-133">String</span></span>|<span data-ttu-id="2c008-134">ユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="2c008-134">User ID</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c008-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2c008-135">Relationships</span></span>
<span data-ttu-id="2c008-136">なし</span><span class="sxs-lookup"><span data-stu-id="2c008-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2c008-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2c008-137">JSON Representation</span></span>
<span data-ttu-id="2c008-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2c008-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.auditActor"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditActor",
  "type": "String",
  "permissions": [
    "String"
  ],
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



