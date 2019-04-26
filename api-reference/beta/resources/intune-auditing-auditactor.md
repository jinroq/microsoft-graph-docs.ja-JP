---
title: auditActor リソースの種類
description: 監査アクターのプロパティが含まれるクラス。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 77150c7a2b883acc6857cd0866459fb9423dfa6c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32558329"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="b1a4a-103">auditActor リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b1a4a-103">auditActor resource type</span></span>

> <span data-ttu-id="b1a4a-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b1a4a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1a4a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b1a4a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1a4a-106">監査アクターのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="b1a4a-106">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="b1a4a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b1a4a-107">Properties</span></span>
|<span data-ttu-id="b1a4a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b1a4a-108">Property</span></span>|<span data-ttu-id="b1a4a-109">型</span><span class="sxs-lookup"><span data-stu-id="b1a4a-109">Type</span></span>|<span data-ttu-id="b1a4a-110">説明</span><span class="sxs-lookup"><span data-stu-id="b1a4a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1a4a-111">type</span><span class="sxs-lookup"><span data-stu-id="b1a4a-111">type</span></span>|<span data-ttu-id="b1a4a-112">String</span><span class="sxs-lookup"><span data-stu-id="b1a4a-112">String</span></span>|<span data-ttu-id="b1a4a-113">アクターの種類。</span><span class="sxs-lookup"><span data-stu-id="b1a4a-113">Actor Type.</span></span>|
|<span data-ttu-id="b1a4a-114">userPermissions</span><span class="sxs-lookup"><span data-stu-id="b1a4a-114">userPermissions</span></span>|<span data-ttu-id="b1a4a-115">String コレクション</span><span class="sxs-lookup"><span data-stu-id="b1a4a-115">String collection</span></span>|<span data-ttu-id="b1a4a-116">監査の実行時におけるユーザーのアクセス許可の一覧。</span><span class="sxs-lookup"><span data-stu-id="b1a4a-116">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="b1a4a-117">applicationId</span><span class="sxs-lookup"><span data-stu-id="b1a4a-117">applicationId</span></span>|<span data-ttu-id="b1a4a-118">String</span><span class="sxs-lookup"><span data-stu-id="b1a4a-118">String</span></span>|<span data-ttu-id="b1a4a-119">AAD アプリケーション ID。</span><span class="sxs-lookup"><span data-stu-id="b1a4a-119">AAD Application Id.</span></span>|
|<span data-ttu-id="b1a4a-120">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="b1a4a-120">applicationDisplayName</span></span>|<span data-ttu-id="b1a4a-121">String</span><span class="sxs-lookup"><span data-stu-id="b1a4a-121">String</span></span>|<span data-ttu-id="b1a4a-122">アプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="b1a4a-122">Name of the Application.</span></span>|
|<span data-ttu-id="b1a4a-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b1a4a-123">userPrincipalName</span></span>|<span data-ttu-id="b1a4a-124">String</span><span class="sxs-lookup"><span data-stu-id="b1a4a-124">String</span></span>|<span data-ttu-id="b1a4a-125">ユーザー プリンシパル名 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="b1a4a-125">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="b1a4a-126">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="b1a4a-126">servicePrincipalName</span></span>|<span data-ttu-id="b1a4a-127">String</span><span class="sxs-lookup"><span data-stu-id="b1a4a-127">String</span></span>|<span data-ttu-id="b1a4a-128">サービス プリンシパル名 (SPN)。</span><span class="sxs-lookup"><span data-stu-id="b1a4a-128">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="b1a4a-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="b1a4a-129">ipAddress</span></span>|<span data-ttu-id="b1a4a-130">String</span><span class="sxs-lookup"><span data-stu-id="b1a4a-130">String</span></span>|<span data-ttu-id="b1a4a-131">IPAddress。</span><span class="sxs-lookup"><span data-stu-id="b1a4a-131">IPAddress.</span></span>|
|<span data-ttu-id="b1a4a-132">userId</span><span class="sxs-lookup"><span data-stu-id="b1a4a-132">userId</span></span>|<span data-ttu-id="b1a4a-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b1a4a-133">String</span></span>|<span data-ttu-id="b1a4a-134">ユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="b1a4a-134">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1a4a-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b1a4a-135">Relationships</span></span>
<span data-ttu-id="b1a4a-136">なし</span><span class="sxs-lookup"><span data-stu-id="b1a4a-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1a4a-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b1a4a-137">JSON Representation</span></span>
<span data-ttu-id="b1a4a-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b1a4a-138">Here is a JSON representation of the resource.</span></span>
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





