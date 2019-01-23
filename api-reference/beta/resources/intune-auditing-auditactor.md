---
title: auditActor リソースの種類
description: 監査アクターのプロパティが含まれるクラス。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fcb9ededd9d1a2bb93f970f9f0da0c41a248e840
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425800"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="32a18-103">auditActor リソースの種類</span><span class="sxs-lookup"><span data-stu-id="32a18-103">auditActor resource type</span></span>

> <span data-ttu-id="32a18-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="32a18-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="32a18-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="32a18-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="32a18-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="32a18-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32a18-107">監査アクターのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="32a18-107">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="32a18-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="32a18-108">Properties</span></span>
|<span data-ttu-id="32a18-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="32a18-109">Property</span></span>|<span data-ttu-id="32a18-110">型</span><span class="sxs-lookup"><span data-stu-id="32a18-110">Type</span></span>|<span data-ttu-id="32a18-111">説明</span><span class="sxs-lookup"><span data-stu-id="32a18-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32a18-112">type</span><span class="sxs-lookup"><span data-stu-id="32a18-112">type</span></span>|<span data-ttu-id="32a18-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="32a18-113">String</span></span>|<span data-ttu-id="32a18-114">アクターの種類。</span><span class="sxs-lookup"><span data-stu-id="32a18-114">Actor Type.</span></span>|
|<span data-ttu-id="32a18-115">userPermissions</span><span class="sxs-lookup"><span data-stu-id="32a18-115">userPermissions</span></span>|<span data-ttu-id="32a18-116">String コレクション</span><span class="sxs-lookup"><span data-stu-id="32a18-116">String collection</span></span>|<span data-ttu-id="32a18-117">監査の実行時におけるユーザーのアクセス許可の一覧。</span><span class="sxs-lookup"><span data-stu-id="32a18-117">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="32a18-118">applicationId</span><span class="sxs-lookup"><span data-stu-id="32a18-118">applicationId</span></span>|<span data-ttu-id="32a18-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="32a18-119">String</span></span>|<span data-ttu-id="32a18-120">AAD アプリケーション ID。</span><span class="sxs-lookup"><span data-stu-id="32a18-120">AAD Application Id.</span></span>|
|<span data-ttu-id="32a18-121">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="32a18-121">applicationDisplayName</span></span>|<span data-ttu-id="32a18-122">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="32a18-122">String</span></span>|<span data-ttu-id="32a18-123">アプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="32a18-123">Name of the Application.</span></span>|
|<span data-ttu-id="32a18-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="32a18-124">userPrincipalName</span></span>|<span data-ttu-id="32a18-125">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="32a18-125">String</span></span>|<span data-ttu-id="32a18-126">ユーザー プリンシパル名 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="32a18-126">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="32a18-127">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="32a18-127">servicePrincipalName</span></span>|<span data-ttu-id="32a18-128">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="32a18-128">String</span></span>|<span data-ttu-id="32a18-129">サービス プリンシパル名 (SPN)。</span><span class="sxs-lookup"><span data-stu-id="32a18-129">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="32a18-130">ipAddress</span><span class="sxs-lookup"><span data-stu-id="32a18-130">ipAddress</span></span>|<span data-ttu-id="32a18-131">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="32a18-131">String</span></span>|<span data-ttu-id="32a18-132">IPAddress。</span><span class="sxs-lookup"><span data-stu-id="32a18-132">IPAddress.</span></span>|
|<span data-ttu-id="32a18-133">userId</span><span class="sxs-lookup"><span data-stu-id="32a18-133">userId</span></span>|<span data-ttu-id="32a18-134">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="32a18-134">String</span></span>|<span data-ttu-id="32a18-135">ユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="32a18-135">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="32a18-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="32a18-136">Relationships</span></span>
<span data-ttu-id="32a18-137">なし</span><span class="sxs-lookup"><span data-stu-id="32a18-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="32a18-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="32a18-138">JSON Representation</span></span>
<span data-ttu-id="32a18-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="32a18-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditActor"
}
-->
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




