---
title: deviceDetail リソースの種類
description: サインインに使用するデバイスに関連付けられているデバイスの詳細を示します。 デバイスが Azure AD で管理されている場合、デバイスブラウザーや OS 情報などの情報が含まれます。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 45d87629f1ac513fe13c98592637f20f5fac0129
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973773"
---
# <a name="devicedetail-resource-type"></a><span data-ttu-id="bd5fd-104">deviceDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bd5fd-104">deviceDetail resource type</span></span>
<span data-ttu-id="bd5fd-105">サインインに使用するデバイスに関連付けられているデバイスの詳細を示します。</span><span class="sxs-lookup"><span data-stu-id="bd5fd-105">Indicates device details associated with a device used for signing in.</span></span> <span data-ttu-id="bd5fd-106">デバイスが Azure AD で管理されている場合、デバイスブラウザーや OS 情報などの情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="bd5fd-106">Includes information like device browser and  OS info, if device is Azure AD managed.</span></span>



## <a name="properties"></a><span data-ttu-id="bd5fd-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bd5fd-107">Properties</span></span>
| <span data-ttu-id="bd5fd-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bd5fd-108">Property</span></span>     | <span data-ttu-id="bd5fd-109">型</span><span class="sxs-lookup"><span data-stu-id="bd5fd-109">Type</span></span>   |<span data-ttu-id="bd5fd-110">説明</span><span class="sxs-lookup"><span data-stu-id="bd5fd-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd5fd-111">ブラウザー</span><span class="sxs-lookup"><span data-stu-id="bd5fd-111">browser</span></span>|<span data-ttu-id="bd5fd-112">String</span><span class="sxs-lookup"><span data-stu-id="bd5fd-112">String</span></span>|<span data-ttu-id="bd5fd-113">サインインに使用するのブラウザー情報を示します。</span><span class="sxs-lookup"><span data-stu-id="bd5fd-113">Indicates the browser information of the used for signing-in.</span></span>|
|<span data-ttu-id="bd5fd-114">deviceId</span><span class="sxs-lookup"><span data-stu-id="bd5fd-114">deviceId</span></span>|<span data-ttu-id="bd5fd-115">String</span><span class="sxs-lookup"><span data-stu-id="bd5fd-115">String</span></span>|<span data-ttu-id="bd5fd-116">サインインに使用されているデバイスの UniqueID を参照します。</span><span class="sxs-lookup"><span data-stu-id="bd5fd-116">Refers to the UniqueID of the device used for signing-in.</span></span>|
|<span data-ttu-id="bd5fd-117">displayName</span><span class="sxs-lookup"><span data-stu-id="bd5fd-117">displayName</span></span>|<span data-ttu-id="bd5fd-118">String</span><span class="sxs-lookup"><span data-stu-id="bd5fd-118">String</span></span>|<span data-ttu-id="bd5fd-119">サインインに使用されているデバイスの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="bd5fd-119">Refers to the name of the device used for signing-in.</span></span>|
|<span data-ttu-id="bd5fd-120">isCompliant</span><span class="sxs-lookup"><span data-stu-id="bd5fd-120">isCompliant</span></span>|<span data-ttu-id="bd5fd-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5fd-121">Boolean</span></span>|<span data-ttu-id="bd5fd-122">デバイスが準拠しているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="bd5fd-122">Indicates whether the device is compliant or not.</span></span>|
|<span data-ttu-id="bd5fd-123">isManaged</span><span class="sxs-lookup"><span data-stu-id="bd5fd-123">isManaged</span></span>|<span data-ttu-id="bd5fd-124">ブール値</span><span class="sxs-lookup"><span data-stu-id="bd5fd-124">Boolean</span></span>|<span data-ttu-id="bd5fd-125">デバイスが管理されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="bd5fd-125">Indicates if the device is managed or not.</span></span>|
|<span data-ttu-id="bd5fd-126">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="bd5fd-126">operatingSystem</span></span>|<span data-ttu-id="bd5fd-127">String</span><span class="sxs-lookup"><span data-stu-id="bd5fd-127">String</span></span>|<span data-ttu-id="bd5fd-128">サインインに使用される OS の名前とバージョンを示します。</span><span class="sxs-lookup"><span data-stu-id="bd5fd-128">Indicates the OS name and version used for signing-in.</span></span>|
|<span data-ttu-id="bd5fd-129">trustType</span><span class="sxs-lookup"><span data-stu-id="bd5fd-129">trustType</span></span>|<span data-ttu-id="bd5fd-130">文字列</span><span class="sxs-lookup"><span data-stu-id="bd5fd-130">String</span></span>|<span data-ttu-id="bd5fd-131">サインインしているデバイスが Workplace Join、AzureAD Join、ドメイン参加しているかどうかについての情報を示します。</span><span class="sxs-lookup"><span data-stu-id="bd5fd-131">Indicates information on whether the signed-in device is Workplace Joined, AzureAD Joined, Domain Joined.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bd5fd-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bd5fd-132">JSON representation</span></span>

<span data-ttu-id="bd5fd-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bd5fd-133">Here is a JSON representation of the resource.</span></span>

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
