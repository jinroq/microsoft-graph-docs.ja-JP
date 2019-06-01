---
title: deviceDetail リソースの種類
description: サインインに使用するデバイスに関連付けられているデバイスの詳細を示します。 デバイスが Azure AD で管理されている場合、デバイスブラウザーや OS 情報などの情報が含まれます。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f3a0d7f141723beb5194860b025fe6fa349eb95a
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657701"
---
# <a name="devicedetail-resource-type"></a><span data-ttu-id="1054c-104">deviceDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1054c-104">deviceDetail resource type</span></span>
<span data-ttu-id="1054c-105">サインインに使用するデバイスに関連付けられているデバイスの詳細を示します。</span><span class="sxs-lookup"><span data-stu-id="1054c-105">Indicates device details associated with a device used for signing in.</span></span> <span data-ttu-id="1054c-106">デバイスが Azure AD で管理されている場合、デバイスブラウザーや OS 情報などの情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="1054c-106">Includes information like device browser and  OS info, if device is Azure AD managed.</span></span>



## <a name="properties"></a><span data-ttu-id="1054c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1054c-107">Properties</span></span>
| <span data-ttu-id="1054c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1054c-108">Property</span></span>     | <span data-ttu-id="1054c-109">型</span><span class="sxs-lookup"><span data-stu-id="1054c-109">Type</span></span>   |<span data-ttu-id="1054c-110">説明</span><span class="sxs-lookup"><span data-stu-id="1054c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1054c-111">ブラウザー</span><span class="sxs-lookup"><span data-stu-id="1054c-111">browser</span></span>|<span data-ttu-id="1054c-112">String</span><span class="sxs-lookup"><span data-stu-id="1054c-112">String</span></span>|<span data-ttu-id="1054c-113">サインインに使用するのブラウザー情報を示します。</span><span class="sxs-lookup"><span data-stu-id="1054c-113">Indicates the browser information of the used for signing-in.</span></span>|
|<span data-ttu-id="1054c-114">deviceId</span><span class="sxs-lookup"><span data-stu-id="1054c-114">deviceId</span></span>|<span data-ttu-id="1054c-115">String</span><span class="sxs-lookup"><span data-stu-id="1054c-115">String</span></span>|<span data-ttu-id="1054c-116">サインインに使用されているデバイスの UniqueID を参照します。</span><span class="sxs-lookup"><span data-stu-id="1054c-116">Refers to the UniqueID of the device used for signing-in.</span></span>|
|<span data-ttu-id="1054c-117">displayName</span><span class="sxs-lookup"><span data-stu-id="1054c-117">displayName</span></span>|<span data-ttu-id="1054c-118">String</span><span class="sxs-lookup"><span data-stu-id="1054c-118">String</span></span>|<span data-ttu-id="1054c-119">サインインに使用されているデバイスの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="1054c-119">Refers to the name of the device used for signing-in.</span></span>|
|<span data-ttu-id="1054c-120">isCompliant</span><span class="sxs-lookup"><span data-stu-id="1054c-120">isCompliant</span></span>|<span data-ttu-id="1054c-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="1054c-121">Boolean</span></span>|<span data-ttu-id="1054c-122">デバイスが準拠しているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1054c-122">Indicates whether the device is compliant or not.</span></span>|
|<span data-ttu-id="1054c-123">isManaged</span><span class="sxs-lookup"><span data-stu-id="1054c-123">isManaged</span></span>|<span data-ttu-id="1054c-124">ブール値</span><span class="sxs-lookup"><span data-stu-id="1054c-124">Boolean</span></span>|<span data-ttu-id="1054c-125">デバイスが管理されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1054c-125">Indicates if the device is managed or not.</span></span>|
|<span data-ttu-id="1054c-126">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="1054c-126">operatingSystem</span></span>|<span data-ttu-id="1054c-127">String</span><span class="sxs-lookup"><span data-stu-id="1054c-127">String</span></span>|<span data-ttu-id="1054c-128">サインインに使用される OS の名前とバージョンを示します。</span><span class="sxs-lookup"><span data-stu-id="1054c-128">Indicates the OS name and version used for signing-in.</span></span>|
|<span data-ttu-id="1054c-129">trustType</span><span class="sxs-lookup"><span data-stu-id="1054c-129">trustType</span></span>|<span data-ttu-id="1054c-130">文字列</span><span class="sxs-lookup"><span data-stu-id="1054c-130">String</span></span>|<span data-ttu-id="1054c-131">サインインしているデバイスが Workplace Join、AzureAD Join、ドメイン参加しているかどうかについての情報を示します。</span><span class="sxs-lookup"><span data-stu-id="1054c-131">Indicates information on whether the signed-in device is Workplace Joined, AzureAD Joined, Domain Joined.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1054c-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1054c-132">JSON representation</span></span>

<span data-ttu-id="1054c-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1054c-133">Here is a JSON representation of the resource.</span></span>

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
