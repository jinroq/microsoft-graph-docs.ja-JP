---
title: managedAppStatusRaw リソースの種類
description: 組織アプリの保護と構成についての型指定されていない進捗レポートを表します。
author: tfitzmac
ms.openlocfilehash: b4cb19b3fd9568afa65b50fea4fb4b3f0c8f1cc4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322695"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="2c873-103">managedAppStatusRaw リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2c873-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="2c873-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2c873-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2c873-105">組織アプリの保護と構成についての型指定されていない進捗レポートを表します。</span><span class="sxs-lookup"><span data-stu-id="2c873-105">Represents an un-typed status report about organizations app protection and configuration.</span></span>

<span data-ttu-id="2c873-106">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2c873-106">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="2c873-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="2c873-107">Methods</span></span>
|<span data-ttu-id="2c873-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="2c873-108">Method</span></span>|<span data-ttu-id="2c873-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2c873-109">Return Type</span></span>|<span data-ttu-id="2c873-110">説明</span><span class="sxs-lookup"><span data-stu-id="2c873-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2c873-111">managedAppStatusRaws のリスト</span><span class="sxs-lookup"><span data-stu-id="2c873-111">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="2c873-112">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2c873-112">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="2c873-113">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="2c873-113">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="2c873-114">managedAppStatusRaw の取得</span><span class="sxs-lookup"><span data-stu-id="2c873-114">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="2c873-115">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="2c873-115">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="2c873-116">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2c873-116">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2c873-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2c873-117">Properties</span></span>
|<span data-ttu-id="2c873-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2c873-118">Property</span></span>|<span data-ttu-id="2c873-119">種類</span><span class="sxs-lookup"><span data-stu-id="2c873-119">Type</span></span>|<span data-ttu-id="2c873-120">説明</span><span class="sxs-lookup"><span data-stu-id="2c873-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c873-121">displayName</span><span class="sxs-lookup"><span data-stu-id="2c873-121">displayName</span></span>|<span data-ttu-id="2c873-122">String</span><span class="sxs-lookup"><span data-stu-id="2c873-122">String</span></span>|<span data-ttu-id="2c873-123">進捗レポートのフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="2c873-123">Friendly name of the status report.</span></span> <span data-ttu-id="2c873-124">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2c873-124">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="2c873-125">id</span><span class="sxs-lookup"><span data-stu-id="2c873-125">id</span></span>|<span data-ttu-id="2c873-126">String</span><span class="sxs-lookup"><span data-stu-id="2c873-126">String</span></span>|<span data-ttu-id="2c873-127">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2c873-127">Key of the entity.</span></span> <span data-ttu-id="2c873-128">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2c873-128">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="2c873-129">version</span><span class="sxs-lookup"><span data-stu-id="2c873-129">version</span></span>|<span data-ttu-id="2c873-130">String</span><span class="sxs-lookup"><span data-stu-id="2c873-130">String</span></span>|<span data-ttu-id="2c873-131">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="2c873-131">Version of the entity.</span></span> <span data-ttu-id="2c873-132">[managedAppStatus](../resources/intune-mam-managedappstatus.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2c873-132">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="2c873-133">content</span><span class="sxs-lookup"><span data-stu-id="2c873-133">content</span></span>|[<span data-ttu-id="2c873-134">Json</span><span class="sxs-lookup"><span data-stu-id="2c873-134">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="2c873-135">進捗レポートの内容。</span><span class="sxs-lookup"><span data-stu-id="2c873-135">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c873-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2c873-136">Relationships</span></span>
<span data-ttu-id="2c873-137">なし</span><span class="sxs-lookup"><span data-stu-id="2c873-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2c873-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2c873-138">JSON Representation</span></span>
<span data-ttu-id="2c873-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2c873-139">Here is a JSON representation of the resource.</span></span>
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



