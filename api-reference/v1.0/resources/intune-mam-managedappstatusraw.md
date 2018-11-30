---
title: managedAppStatusRaw リソースの種類
description: 組織アプリの保護と構成についての型指定されていない進捗レポートを表します。
ms.openlocfilehash: 9576123e39be2ae37052926342fb634c21086371
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023298"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="f82cd-103">managedAppStatusRaw リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f82cd-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="f82cd-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f82cd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f82cd-105">組織アプリの保護と構成についての型指定されていない進捗レポートを表します。</span><span class="sxs-lookup"><span data-stu-id="f82cd-105">Represents an un-typed status report about organizations app protection and configuration.</span></span>

<span data-ttu-id="f82cd-106">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f82cd-106">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="f82cd-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="f82cd-107">Methods</span></span>
|<span data-ttu-id="f82cd-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="f82cd-108">Method</span></span>|<span data-ttu-id="f82cd-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f82cd-109">Return Type</span></span>|<span data-ttu-id="f82cd-110">説明</span><span class="sxs-lookup"><span data-stu-id="f82cd-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f82cd-111">managedAppStatusRaws のリスト</span><span class="sxs-lookup"><span data-stu-id="f82cd-111">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="f82cd-112">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f82cd-112">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="f82cd-113">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="f82cd-113">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="f82cd-114">managedAppStatusRaw の取得</span><span class="sxs-lookup"><span data-stu-id="f82cd-114">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="f82cd-115">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="f82cd-115">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="f82cd-116">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f82cd-116">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f82cd-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f82cd-117">Properties</span></span>
|<span data-ttu-id="f82cd-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f82cd-118">Property</span></span>|<span data-ttu-id="f82cd-119">型</span><span class="sxs-lookup"><span data-stu-id="f82cd-119">Type</span></span>|<span data-ttu-id="f82cd-120">説明</span><span class="sxs-lookup"><span data-stu-id="f82cd-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f82cd-121">displayName</span><span class="sxs-lookup"><span data-stu-id="f82cd-121">displayName</span></span>|<span data-ttu-id="f82cd-122">String</span><span class="sxs-lookup"><span data-stu-id="f82cd-122">String</span></span>|<span data-ttu-id="f82cd-123">進捗レポートのフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="f82cd-123">Friendly name of the status report.</span></span> <span data-ttu-id="f82cd-124">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f82cd-124">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="f82cd-125">id</span><span class="sxs-lookup"><span data-stu-id="f82cd-125">id</span></span>|<span data-ttu-id="f82cd-126">String</span><span class="sxs-lookup"><span data-stu-id="f82cd-126">String</span></span>|<span data-ttu-id="f82cd-127">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f82cd-127">Key of the entity.</span></span> <span data-ttu-id="f82cd-128">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f82cd-128">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="f82cd-129">version</span><span class="sxs-lookup"><span data-stu-id="f82cd-129">version</span></span>|<span data-ttu-id="f82cd-130">String</span><span class="sxs-lookup"><span data-stu-id="f82cd-130">String</span></span>|<span data-ttu-id="f82cd-131">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="f82cd-131">Version of the entity.</span></span> <span data-ttu-id="f82cd-132">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f82cd-132">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="f82cd-133">content</span><span class="sxs-lookup"><span data-stu-id="f82cd-133">content</span></span>|[<span data-ttu-id="f82cd-134">Json</span><span class="sxs-lookup"><span data-stu-id="f82cd-134">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="f82cd-135">進捗レポートの内容。</span><span class="sxs-lookup"><span data-stu-id="f82cd-135">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f82cd-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f82cd-136">Relationships</span></span>
<span data-ttu-id="f82cd-137">なし</span><span class="sxs-lookup"><span data-stu-id="f82cd-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f82cd-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f82cd-138">JSON Representation</span></span>
<span data-ttu-id="f82cd-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f82cd-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatusRaw"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatusRaw",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```



