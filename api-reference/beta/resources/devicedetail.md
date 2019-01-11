---
title: deviceDetail リソースの種類
description: サインインに使用するデバイスに関連付けられているデバイスの詳細を示します。 デバイスが管理される Azure の AD の場合は、デバイスのブラウザーおよび OS の情報などの情報に含まれています。
localization_priority: Normal
ms.openlocfilehash: ca4679a8c484b6dc5b36ef39d3d6d039537cbdbb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884841"
---
# <a name="devicedetail-resource-type"></a><span data-ttu-id="c7253-104">deviceDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c7253-104">deviceDetail resource type</span></span>
<span data-ttu-id="c7253-105">サインインに使用するデバイスに関連付けられているデバイスの詳細を示します。</span><span class="sxs-lookup"><span data-stu-id="c7253-105">Indicates device details associated with a device used for signing in.</span></span> <span data-ttu-id="c7253-106">デバイスが管理される Azure の AD の場合は、デバイスのブラウザーおよび OS の情報などの情報に含まれています。</span><span class="sxs-lookup"><span data-stu-id="c7253-106">Includes information like device browser and  OS info, if device is Azure AD managed.</span></span>



## <a name="properties"></a><span data-ttu-id="c7253-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c7253-107">Properties</span></span>
| <span data-ttu-id="c7253-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c7253-108">Property</span></span>     | <span data-ttu-id="c7253-109">種類</span><span class="sxs-lookup"><span data-stu-id="c7253-109">Type</span></span>   |<span data-ttu-id="c7253-110">説明</span><span class="sxs-lookup"><span data-stu-id="c7253-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c7253-111">ブラウザー</span><span class="sxs-lookup"><span data-stu-id="c7253-111">browser</span></span>|<span data-ttu-id="c7253-112">String</span><span class="sxs-lookup"><span data-stu-id="c7253-112">String</span></span>|<span data-ttu-id="c7253-113">使用のブラウザー情報の署名に。</span><span class="sxs-lookup"><span data-stu-id="c7253-113">Indicates the browser information of the used for signing-in.</span></span>|
|<span data-ttu-id="c7253-114">deviceId</span><span class="sxs-lookup"><span data-stu-id="c7253-114">deviceId</span></span>|<span data-ttu-id="c7253-115">String</span><span class="sxs-lookup"><span data-stu-id="c7253-115">String</span></span>|<span data-ttu-id="c7253-116">署名に使用するデバイスの UniqueID を意味します。</span><span class="sxs-lookup"><span data-stu-id="c7253-116">Refers to the UniqueID of the device used for signing-in.</span></span>|
|<span data-ttu-id="c7253-117">displayName</span><span class="sxs-lookup"><span data-stu-id="c7253-117">displayName</span></span>|<span data-ttu-id="c7253-118">String</span><span class="sxs-lookup"><span data-stu-id="c7253-118">String</span></span>|<span data-ttu-id="c7253-119">署名に使用するデバイスの名前を参照します。</span><span class="sxs-lookup"><span data-stu-id="c7253-119">Refers to the name of the device used for signing-in.</span></span>|
|<span data-ttu-id="c7253-120">isCompliant</span><span class="sxs-lookup"><span data-stu-id="c7253-120">isCompliant</span></span>|<span data-ttu-id="c7253-121">ブール値</span><span class="sxs-lookup"><span data-stu-id="c7253-121">Boolean</span></span>|<span data-ttu-id="c7253-122">デバイスが準拠しているかどうかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c7253-122">Indicates whether the device is compliant or not.</span></span>|
|<span data-ttu-id="c7253-123">isManaged</span><span class="sxs-lookup"><span data-stu-id="c7253-123">isManaged</span></span>|<span data-ttu-id="c7253-124">ブール値</span><span class="sxs-lookup"><span data-stu-id="c7253-124">Boolean</span></span>|<span data-ttu-id="c7253-125">か、デバイスが管理されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="c7253-125">Indicates if the device is managed or not.</span></span>|
|<span data-ttu-id="c7253-126">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="c7253-126">operatingSystem</span></span>|<span data-ttu-id="c7253-127">String</span><span class="sxs-lookup"><span data-stu-id="c7253-127">String</span></span>|<span data-ttu-id="c7253-128">OS の名前と署名に使用されるバージョンを示します。</span><span class="sxs-lookup"><span data-stu-id="c7253-128">Indicates the OS name and version used for signing-in.</span></span>|
|<span data-ttu-id="c7253-129">trustType</span><span class="sxs-lookup"><span data-stu-id="c7253-129">trustType</span></span>|<span data-ttu-id="c7253-130">String</span><span class="sxs-lookup"><span data-stu-id="c7253-130">String</span></span>|<span data-ttu-id="c7253-131">署名付きのデバイスは、ワークプ レースに参加して、AzureAD に参加して、ドメインに参加しているかどうかに関する情報を示します。</span><span class="sxs-lookup"><span data-stu-id="c7253-131">Indicates information on whether the signed-in device is Workplace Joined, AzureAD Joined, Domain Joined.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c7253-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c7253-132">JSON representation</span></span>

<span data-ttu-id="c7253-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c7253-133">Here is a JSON representation of the resource.</span></span>

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
