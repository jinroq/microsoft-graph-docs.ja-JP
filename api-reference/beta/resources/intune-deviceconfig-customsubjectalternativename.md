---
title: Customsubjectoff・ベンダーのリソースの種類
description: カスタムサブジェクトの別名定義
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cf3c7a8e675c41056b1c5450b83394951b2ceab4
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947403"
---
# <a name="customsubjectalternativename-resource-type"></a><span data-ttu-id="ffc1f-103">Customsubjectoff・ベンダーのリソースの種類</span><span class="sxs-lookup"><span data-stu-id="ffc1f-103">customSubjectAlternativeName resource type</span></span>

> <span data-ttu-id="ffc1f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ffc1f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ffc1f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ffc1f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffc1f-106">カスタムサブジェクトの別名定義</span><span class="sxs-lookup"><span data-stu-id="ffc1f-106">Custom Subject Alternative Name definition</span></span>

## <a name="properties"></a><span data-ttu-id="ffc1f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ffc1f-107">Properties</span></span>
|<span data-ttu-id="ffc1f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ffc1f-108">Property</span></span>|<span data-ttu-id="ffc1f-109">型</span><span class="sxs-lookup"><span data-stu-id="ffc1f-109">Type</span></span>|<span data-ttu-id="ffc1f-110">説明</span><span class="sxs-lookup"><span data-stu-id="ffc1f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffc1f-111">sanType</span><span class="sxs-lookup"><span data-stu-id="ffc1f-111">sanType</span></span>|[<span data-ttu-id="ffc1f-112">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="ffc1f-112">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="ffc1f-113">カスタム SAN の種類。</span><span class="sxs-lookup"><span data-stu-id="ffc1f-113">Custom SAN Type.</span></span> <span data-ttu-id="ffc1f-114">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="ffc1f-114">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="ffc1f-115">name</span><span class="sxs-lookup"><span data-stu-id="ffc1f-115">name</span></span>|<span data-ttu-id="ffc1f-116">String</span><span class="sxs-lookup"><span data-stu-id="ffc1f-116">String</span></span>|<span data-ttu-id="ffc1f-117">ユーザー設定の SAN 名</span><span class="sxs-lookup"><span data-stu-id="ffc1f-117">Custom SAN Name</span></span>|

## <a name="relationships"></a><span data-ttu-id="ffc1f-118">関係</span><span class="sxs-lookup"><span data-stu-id="ffc1f-118">Relationships</span></span>
<span data-ttu-id="ffc1f-119">なし</span><span class="sxs-lookup"><span data-stu-id="ffc1f-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ffc1f-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ffc1f-120">JSON Representation</span></span>
<span data-ttu-id="ffc1f-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ffc1f-121">Here is a JSON representation of the resource.</span></span>
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




