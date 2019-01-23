---
title: customSubjectAlternativeName リソースの種類
description: カスタムのサブジェクトの別名定義
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b3f081b37b79be45d6705d24be58ea7295b58b68
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415671"
---
# <a name="customsubjectalternativename-resource-type"></a><span data-ttu-id="fba68-103">customSubjectAlternativeName リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fba68-103">customSubjectAlternativeName resource type</span></span>

> <span data-ttu-id="fba68-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fba68-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fba68-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fba68-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fba68-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fba68-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fba68-107">カスタムのサブジェクトの別名定義</span><span class="sxs-lookup"><span data-stu-id="fba68-107">Custom Subject Alternative Name definition</span></span>

## <a name="properties"></a><span data-ttu-id="fba68-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fba68-108">Properties</span></span>
|<span data-ttu-id="fba68-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fba68-109">Property</span></span>|<span data-ttu-id="fba68-110">型</span><span class="sxs-lookup"><span data-stu-id="fba68-110">Type</span></span>|<span data-ttu-id="fba68-111">説明</span><span class="sxs-lookup"><span data-stu-id="fba68-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fba68-112">sanType</span><span class="sxs-lookup"><span data-stu-id="fba68-112">sanType</span></span>|[<span data-ttu-id="fba68-113">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="fba68-113">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="fba68-114">SAN のカスタム型です。</span><span class="sxs-lookup"><span data-stu-id="fba68-114">Custom SAN Type.</span></span> <span data-ttu-id="fba68-115">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="fba68-115">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="fba68-116">name</span><span class="sxs-lookup"><span data-stu-id="fba68-116">name</span></span>|<span data-ttu-id="fba68-117">String</span><span class="sxs-lookup"><span data-stu-id="fba68-117">String</span></span>|<span data-ttu-id="fba68-118">SAN のカスタム名</span><span class="sxs-lookup"><span data-stu-id="fba68-118">Custom SAN Name</span></span>|

## <a name="relationships"></a><span data-ttu-id="fba68-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fba68-119">Relationships</span></span>
<span data-ttu-id="fba68-120">なし</span><span class="sxs-lookup"><span data-stu-id="fba68-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fba68-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fba68-121">JSON Representation</span></span>
<span data-ttu-id="fba68-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fba68-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customSubjectAlternativeName"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customSubjectAlternativeName",
  "sanType": "String",
  "name": "String"
}
```




