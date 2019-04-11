---
title: customsubjectoff・ベンダーのリソースの種類
description: カスタムサブジェクトの別名定義
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 03507d4e912af011db011283a95887590ab79801
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31783952"
---
# <a name="customsubjectalternativename-resource-type"></a><span data-ttu-id="bf755-103">customsubjectoff・ベンダーのリソースの種類</span><span class="sxs-lookup"><span data-stu-id="bf755-103">customSubjectAlternativeName resource type</span></span>

> <span data-ttu-id="bf755-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bf755-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf755-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bf755-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf755-106">カスタムサブジェクトの別名定義</span><span class="sxs-lookup"><span data-stu-id="bf755-106">Custom Subject Alternative Name definition</span></span>

## <a name="properties"></a><span data-ttu-id="bf755-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf755-107">Properties</span></span>
|<span data-ttu-id="bf755-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf755-108">Property</span></span>|<span data-ttu-id="bf755-109">型</span><span class="sxs-lookup"><span data-stu-id="bf755-109">Type</span></span>|<span data-ttu-id="bf755-110">説明</span><span class="sxs-lookup"><span data-stu-id="bf755-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf755-111">santype</span><span class="sxs-lookup"><span data-stu-id="bf755-111">sanType</span></span>|[<span data-ttu-id="bf755-112">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="bf755-112">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="bf755-113">カスタム SAN の種類。</span><span class="sxs-lookup"><span data-stu-id="bf755-113">Custom SAN Type.</span></span> <span data-ttu-id="bf755-114">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="bf755-114">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="bf755-115">name</span><span class="sxs-lookup"><span data-stu-id="bf755-115">name</span></span>|<span data-ttu-id="bf755-116">String</span><span class="sxs-lookup"><span data-stu-id="bf755-116">String</span></span>|<span data-ttu-id="bf755-117">ユーザー設定の SAN 名</span><span class="sxs-lookup"><span data-stu-id="bf755-117">Custom SAN Name</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf755-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bf755-118">Relationships</span></span>
<span data-ttu-id="bf755-119">なし</span><span class="sxs-lookup"><span data-stu-id="bf755-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf755-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bf755-120">JSON Representation</span></span>
<span data-ttu-id="bf755-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bf755-121">Here is a JSON representation of the resource.</span></span>
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





