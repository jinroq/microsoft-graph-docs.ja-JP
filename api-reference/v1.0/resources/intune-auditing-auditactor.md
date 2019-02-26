---
title: auditActor リソースの種類
description: 監査アクターのプロパティが含まれるクラス。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 632e3018f606b62171461b4b1235ccdafc6b1b5a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254458"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="c1e72-103">auditActor リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c1e72-103">auditActor resource type</span></span>

> <span data-ttu-id="c1e72-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c1e72-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1e72-105">監査アクターのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="c1e72-105">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="c1e72-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1e72-106">Properties</span></span>
|<span data-ttu-id="c1e72-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1e72-107">Property</span></span>|<span data-ttu-id="c1e72-108">型</span><span class="sxs-lookup"><span data-stu-id="c1e72-108">Type</span></span>|<span data-ttu-id="c1e72-109">説明</span><span class="sxs-lookup"><span data-stu-id="c1e72-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1e72-110">type</span><span class="sxs-lookup"><span data-stu-id="c1e72-110">type</span></span>|<span data-ttu-id="c1e72-111">String</span><span class="sxs-lookup"><span data-stu-id="c1e72-111">String</span></span>|<span data-ttu-id="c1e72-112">アクターの種類。</span><span class="sxs-lookup"><span data-stu-id="c1e72-112">Actor Type.</span></span>|
|<span data-ttu-id="c1e72-113">userPermissions</span><span class="sxs-lookup"><span data-stu-id="c1e72-113">userPermissions</span></span>|<span data-ttu-id="c1e72-114">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c1e72-114">String collection</span></span>|<span data-ttu-id="c1e72-115">監査の実行時におけるユーザーのアクセス許可の一覧。</span><span class="sxs-lookup"><span data-stu-id="c1e72-115">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="c1e72-116">applicationId</span><span class="sxs-lookup"><span data-stu-id="c1e72-116">applicationId</span></span>|<span data-ttu-id="c1e72-117">String</span><span class="sxs-lookup"><span data-stu-id="c1e72-117">String</span></span>|<span data-ttu-id="c1e72-118">AAD アプリケーション ID。</span><span class="sxs-lookup"><span data-stu-id="c1e72-118">AAD Application Id.</span></span>|
|<span data-ttu-id="c1e72-119">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="c1e72-119">applicationDisplayName</span></span>|<span data-ttu-id="c1e72-120">String</span><span class="sxs-lookup"><span data-stu-id="c1e72-120">String</span></span>|<span data-ttu-id="c1e72-121">アプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="c1e72-121">Name of the Application.</span></span>|
|<span data-ttu-id="c1e72-122">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c1e72-122">userPrincipalName</span></span>|<span data-ttu-id="c1e72-123">文字列</span><span class="sxs-lookup"><span data-stu-id="c1e72-123">String</span></span>|<span data-ttu-id="c1e72-124">ユーザー プリンシパル名 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="c1e72-124">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="c1e72-125">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="c1e72-125">servicePrincipalName</span></span>|<span data-ttu-id="c1e72-126">String</span><span class="sxs-lookup"><span data-stu-id="c1e72-126">String</span></span>|<span data-ttu-id="c1e72-127">サービス プリンシパル名 (SPN)。</span><span class="sxs-lookup"><span data-stu-id="c1e72-127">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="c1e72-128">ipAddress</span><span class="sxs-lookup"><span data-stu-id="c1e72-128">ipAddress</span></span>|<span data-ttu-id="c1e72-129">String</span><span class="sxs-lookup"><span data-stu-id="c1e72-129">String</span></span>|<span data-ttu-id="c1e72-130">IPAddress。</span><span class="sxs-lookup"><span data-stu-id="c1e72-130">IPAddress.</span></span>|
|<span data-ttu-id="c1e72-131">userId</span><span class="sxs-lookup"><span data-stu-id="c1e72-131">userId</span></span>|<span data-ttu-id="c1e72-132">String</span><span class="sxs-lookup"><span data-stu-id="c1e72-132">String</span></span>|<span data-ttu-id="c1e72-133">ユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="c1e72-133">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1e72-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c1e72-134">Relationships</span></span>
<span data-ttu-id="c1e72-135">なし</span><span class="sxs-lookup"><span data-stu-id="c1e72-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1e72-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c1e72-136">JSON Representation</span></span>
<span data-ttu-id="c1e72-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c1e72-137">Here is a JSON representation of the resource.</span></span>
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



