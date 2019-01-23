---
title: windowsInformationProtectionDataRecoveryCertificate リソースの種類
description: Windows 情報保護の DataRecoveryCertificate
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f6a5606906cbec0122137faf3cb454edec785c42
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405801"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="68bb3-103">windowsInformationProtectionDataRecoveryCertificate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="68bb3-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="68bb3-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="68bb3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="68bb3-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="68bb3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="68bb3-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="68bb3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68bb3-107">Windows 情報保護の DataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="68bb3-107">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="68bb3-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="68bb3-108">Properties</span></span>
|<span data-ttu-id="68bb3-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="68bb3-109">Property</span></span>|<span data-ttu-id="68bb3-110">型</span><span class="sxs-lookup"><span data-stu-id="68bb3-110">Type</span></span>|<span data-ttu-id="68bb3-111">説明</span><span class="sxs-lookup"><span data-stu-id="68bb3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68bb3-112">subjectName</span><span class="sxs-lookup"><span data-stu-id="68bb3-112">subjectName</span></span>|<span data-ttu-id="68bb3-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="68bb3-113">String</span></span>|<span data-ttu-id="68bb3-114">データ回復証明書のサブジェクト名</span><span class="sxs-lookup"><span data-stu-id="68bb3-114">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="68bb3-115">説明</span><span class="sxs-lookup"><span data-stu-id="68bb3-115">description</span></span>|<span data-ttu-id="68bb3-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="68bb3-116">String</span></span>|<span data-ttu-id="68bb3-117">データ回復証明書の説明</span><span class="sxs-lookup"><span data-stu-id="68bb3-117">Data recovery Certificate description</span></span>|
|<span data-ttu-id="68bb3-118">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="68bb3-118">expirationDateTime</span></span>|<span data-ttu-id="68bb3-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68bb3-119">DateTimeOffset</span></span>|<span data-ttu-id="68bb3-120">データ回復証明書の有効期限日時</span><span class="sxs-lookup"><span data-stu-id="68bb3-120">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="68bb3-121">certificate</span><span class="sxs-lookup"><span data-stu-id="68bb3-121">certificate</span></span>|<span data-ttu-id="68bb3-122">バイナリ型 (Binary)</span><span class="sxs-lookup"><span data-stu-id="68bb3-122">Binary</span></span>|<span data-ttu-id="68bb3-123">データ回復証明書</span><span class="sxs-lookup"><span data-stu-id="68bb3-123">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="68bb3-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="68bb3-124">Relationships</span></span>
<span data-ttu-id="68bb3-125">なし</span><span class="sxs-lookup"><span data-stu-id="68bb3-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="68bb3-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="68bb3-126">JSON Representation</span></span>
<span data-ttu-id="68bb3-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="68bb3-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
  "subjectName": "String",
  "description": "String",
  "expirationDateTime": "String (timestamp)",
  "certificate": "binary"
}
```




