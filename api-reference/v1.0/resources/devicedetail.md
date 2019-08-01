---
title: deviceDetail リソースの種類
description: サインインに使用するデバイスに関連付けられているデバイスの詳細を示します。 これには、デバイスブラウザーとオペレーティングシステム、デバイスが Azure AD で管理されているかどうかなどの情報が含まれます。
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7cf5de980f28768fdd92ed4b052e0c678be1cdac
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029499"
---
# <a name="devicedetail-resource-type"></a><span data-ttu-id="46efc-104">deviceDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="46efc-104">deviceDetail resource type</span></span>

<span data-ttu-id="46efc-105">サインインに使用するデバイスに関連付けられているデバイスの詳細を示します。</span><span class="sxs-lookup"><span data-stu-id="46efc-105">Indicates device details associated with a device used for signing in.</span></span> <span data-ttu-id="46efc-106">これには、デバイスブラウザーとオペレーティングシステム、デバイスが Azure AD で管理されているかどうかなどの情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="46efc-106">This includes information like device browser and  operating system, and whether the device is Azure AD managed.</span></span>

## <a name="properties"></a><span data-ttu-id="46efc-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="46efc-107">Properties</span></span>

| <span data-ttu-id="46efc-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="46efc-108">Property</span></span>     | <span data-ttu-id="46efc-109">型</span><span class="sxs-lookup"><span data-stu-id="46efc-109">Type</span></span>   |<span data-ttu-id="46efc-110">説明</span><span class="sxs-lookup"><span data-stu-id="46efc-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46efc-111">ブラウザー</span><span class="sxs-lookup"><span data-stu-id="46efc-111">browser</span></span>|<span data-ttu-id="46efc-112">String</span><span class="sxs-lookup"><span data-stu-id="46efc-112">String</span></span>|<span data-ttu-id="46efc-113">サインインに使用するのブラウザー情報を示します。</span><span class="sxs-lookup"><span data-stu-id="46efc-113">Indicates the browser information of the used for signing in.</span></span>|
|<span data-ttu-id="46efc-114">deviceId</span><span class="sxs-lookup"><span data-stu-id="46efc-114">deviceId</span></span>|<span data-ttu-id="46efc-115">String</span><span class="sxs-lookup"><span data-stu-id="46efc-115">String</span></span>|<span data-ttu-id="46efc-116">サインインに使用されているデバイスの UniqueID を参照します。</span><span class="sxs-lookup"><span data-stu-id="46efc-116">Refers to the UniqueID of the device used for signing in.</span></span>|
|<span data-ttu-id="46efc-117">displayName</span><span class="sxs-lookup"><span data-stu-id="46efc-117">displayName</span></span>|<span data-ttu-id="46efc-118">String</span><span class="sxs-lookup"><span data-stu-id="46efc-118">String</span></span>|<span data-ttu-id="46efc-119">サインインに使用されているデバイスの名前を参照します。</span><span class="sxs-lookup"><span data-stu-id="46efc-119">Refers to the name of the device used for signing in.</span></span>|
|<span data-ttu-id="46efc-120">isCompliant</span><span class="sxs-lookup"><span data-stu-id="46efc-120">isCompliant</span></span>|<span data-ttu-id="46efc-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="46efc-121">Boolean</span></span>|<span data-ttu-id="46efc-122">デバイスが準拠しているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="46efc-122">Indicates whether the device is compliant.</span></span>|
|<span data-ttu-id="46efc-123">isManaged</span><span class="sxs-lookup"><span data-stu-id="46efc-123">isManaged</span></span>|<span data-ttu-id="46efc-124">ブール値</span><span class="sxs-lookup"><span data-stu-id="46efc-124">Boolean</span></span>|<span data-ttu-id="46efc-125">デバイスが管理されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="46efc-125">Indicates whether the device is managed.</span></span>|
|<span data-ttu-id="46efc-126">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="46efc-126">operatingSystem</span></span>|<span data-ttu-id="46efc-127">String</span><span class="sxs-lookup"><span data-stu-id="46efc-127">String</span></span>|<span data-ttu-id="46efc-128">サインインに使用するオペレーティングシステムの名前とバージョンを示します。</span><span class="sxs-lookup"><span data-stu-id="46efc-128">Indicates the operating system name and version used for signing in.</span></span>|
|<span data-ttu-id="46efc-129">trustType</span><span class="sxs-lookup"><span data-stu-id="46efc-129">trustType</span></span>|<span data-ttu-id="46efc-130">文字列</span><span class="sxs-lookup"><span data-stu-id="46efc-130">String</span></span>|<span data-ttu-id="46efc-131">サインインしているデバイスが、Workplace Join、AzureAD Join、ドメインに参加しているかどうかに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="46efc-131">Provides information about whether the signed-in device is Workplace Joined, AzureAD Joined, Domain Joined.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="46efc-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="46efc-132">JSON representation</span></span>

<span data-ttu-id="46efc-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="46efc-133">Here is a JSON representation of the resource.</span></span>

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
