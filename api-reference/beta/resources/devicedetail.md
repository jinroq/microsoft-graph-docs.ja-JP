---
title: deviceDetail リソースの種類
description: サインインに使用するデバイスに関連付けられているデバイスの詳細を示します。 デバイスが管理される Azure の AD の場合は、デバイスのブラウザーおよび OS の情報などの情報に含まれています。
ms.openlocfilehash: d7c1830ee5c99fc139a937fcee3896e2a9926592
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067473"
---
# <a name="devicedetail-resource-type"></a><span data-ttu-id="89da9-104">deviceDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="89da9-104">deviceDetail resource type</span></span>
<span data-ttu-id="89da9-105">サインインに使用するデバイスに関連付けられているデバイスの詳細を示します。</span><span class="sxs-lookup"><span data-stu-id="89da9-105">Indicates device details associated with a device used for signing in.</span></span> <span data-ttu-id="89da9-106">デバイスが管理される Azure の AD の場合は、デバイスのブラウザーおよび OS の情報などの情報に含まれています。</span><span class="sxs-lookup"><span data-stu-id="89da9-106">Includes information like device browser and  OS info, if device is Azure AD managed.</span></span>



## <a name="properties"></a><span data-ttu-id="89da9-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="89da9-107">Properties</span></span>
| <span data-ttu-id="89da9-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="89da9-108">Property</span></span>     | <span data-ttu-id="89da9-109">型</span><span class="sxs-lookup"><span data-stu-id="89da9-109">Type</span></span>   |<span data-ttu-id="89da9-110">説明</span><span class="sxs-lookup"><span data-stu-id="89da9-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89da9-111">ブラウザー</span><span class="sxs-lookup"><span data-stu-id="89da9-111">browser</span></span>|<span data-ttu-id="89da9-112">String</span><span class="sxs-lookup"><span data-stu-id="89da9-112">String</span></span>|<span data-ttu-id="89da9-113">使用のブラウザー情報の署名に。</span><span class="sxs-lookup"><span data-stu-id="89da9-113">Indicates the browser information of the used for signing-in.</span></span>|
|<span data-ttu-id="89da9-114">deviceId</span><span class="sxs-lookup"><span data-stu-id="89da9-114">deviceId</span></span>|<span data-ttu-id="89da9-115">String</span><span class="sxs-lookup"><span data-stu-id="89da9-115">String</span></span>|<span data-ttu-id="89da9-116">署名に使用するデバイスの UniqueID を意味します。</span><span class="sxs-lookup"><span data-stu-id="89da9-116">Refers to the UniqueID of the device used for signing-in.</span></span>|
|<span data-ttu-id="89da9-117">displayName</span><span class="sxs-lookup"><span data-stu-id="89da9-117">displayName</span></span>|<span data-ttu-id="89da9-118">String</span><span class="sxs-lookup"><span data-stu-id="89da9-118">String</span></span>|<span data-ttu-id="89da9-119">署名に使用するデバイスの名前を参照します。</span><span class="sxs-lookup"><span data-stu-id="89da9-119">Refers to the name of the device used for signing-in.</span></span>|
|<span data-ttu-id="89da9-120">isCompliant</span><span class="sxs-lookup"><span data-stu-id="89da9-120">isCompliant</span></span>|<span data-ttu-id="89da9-121">ブール値</span><span class="sxs-lookup"><span data-stu-id="89da9-121">Boolean</span></span>|<span data-ttu-id="89da9-122">デバイスが準拠しているかどうかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="89da9-122">Indicates whether the device is compliant or not.</span></span>|
|<span data-ttu-id="89da9-123">isManaged</span><span class="sxs-lookup"><span data-stu-id="89da9-123">isManaged</span></span>|<span data-ttu-id="89da9-124">ブール値</span><span class="sxs-lookup"><span data-stu-id="89da9-124">Boolean</span></span>|<span data-ttu-id="89da9-125">か、デバイスが管理されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="89da9-125">Indicates if the device is managed or not.</span></span>|
|<span data-ttu-id="89da9-126">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="89da9-126">operatingSystem</span></span>|<span data-ttu-id="89da9-127">String</span><span class="sxs-lookup"><span data-stu-id="89da9-127">String</span></span>|<span data-ttu-id="89da9-128">OS の名前と署名に使用されるバージョンを示します。</span><span class="sxs-lookup"><span data-stu-id="89da9-128">Indicates the OS name and version used for signing-in.</span></span>|
|<span data-ttu-id="89da9-129">trustType</span><span class="sxs-lookup"><span data-stu-id="89da9-129">trustType</span></span>|<span data-ttu-id="89da9-130">String</span><span class="sxs-lookup"><span data-stu-id="89da9-130">String</span></span>|<span data-ttu-id="89da9-131">署名付きのデバイスは、ワークプ レースに参加して、AzureAD に参加して、ドメインに参加しているかどうかに関する情報を示します。</span><span class="sxs-lookup"><span data-stu-id="89da9-131">Indicates information on whether the signed-in device is Workplace Joined, AzureAD Joined, Domain Joined.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="89da9-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="89da9-132">JSON representation</span></span>

<span data-ttu-id="89da9-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="89da9-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.deviceDetail"
}-->

```json
{
  "browser": "String",
  "deviceId": "String",
  "displayName": "String",
  "isCompliant": true,
  "isManaged": true,
  "operatingSystem": "String",
  "trustType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "deviceDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->