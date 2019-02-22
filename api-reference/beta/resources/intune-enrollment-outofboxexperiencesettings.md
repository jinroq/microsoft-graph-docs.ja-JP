---
title: outOfBoxExperienceSettings リソースの種類
description: 不在時の環境設定
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1148ba609a6533dcc6cedb9abd50e9191dceb5d2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145529"
---
# <a name="outofboxexperiencesettings-resource-type"></a><span data-ttu-id="f0bdb-103">outOfBoxExperienceSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f0bdb-103">outOfBoxExperienceSettings resource type</span></span>

> <span data-ttu-id="f0bdb-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0bdb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0bdb-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f0bdb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0bdb-106">不在時の環境設定</span><span class="sxs-lookup"><span data-stu-id="f0bdb-106">Out of box experience setting</span></span>

## <a name="properties"></a><span data-ttu-id="f0bdb-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f0bdb-107">Properties</span></span>
|<span data-ttu-id="f0bdb-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f0bdb-108">Property</span></span>|<span data-ttu-id="f0bdb-109">型</span><span class="sxs-lookup"><span data-stu-id="f0bdb-109">Type</span></span>|<span data-ttu-id="f0bdb-110">説明</span><span class="sxs-lookup"><span data-stu-id="f0bdb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0bdb-111">hideprivacysettings</span><span class="sxs-lookup"><span data-stu-id="f0bdb-111">hidePrivacySettings</span></span>|<span data-ttu-id="f0bdb-112">ブール値</span><span class="sxs-lookup"><span data-stu-id="f0bdb-112">Boolean</span></span>|<span data-ttu-id="f0bdb-113">ユーザーのプライバシー設定を表示または非表示にする</span><span class="sxs-lookup"><span data-stu-id="f0bdb-113">Show or hide privacy settings to user</span></span>|
|<span data-ttu-id="f0bdb-114">hideeula</span><span class="sxs-lookup"><span data-stu-id="f0bdb-114">hideEULA</span></span>|<span data-ttu-id="f0bdb-115">ブール値</span><span class="sxs-lookup"><span data-stu-id="f0bdb-115">Boolean</span></span>|<span data-ttu-id="f0bdb-116">ユーザーに EULA を表示または非表示にする</span><span class="sxs-lookup"><span data-stu-id="f0bdb-116">Show or hide EULA to user</span></span>|
|<span data-ttu-id="f0bdb-117">userType</span><span class="sxs-lookup"><span data-stu-id="f0bdb-117">userType</span></span>|[<span data-ttu-id="f0bdb-118">windowsUserType</span><span class="sxs-lookup"><span data-stu-id="f0bdb-118">windowsUserType</span></span>](../resources/intune-enrollment-windowsusertype.md)|<span data-ttu-id="f0bdb-119">ユーザーの種類。</span><span class="sxs-lookup"><span data-stu-id="f0bdb-119">Type of user.</span></span> <span data-ttu-id="f0bdb-120">使用可能な値は、`administrator`、`standard` です。</span><span class="sxs-lookup"><span data-stu-id="f0bdb-120">Possible values are: `administrator`, `standard`.</span></span>|
|<span data-ttu-id="f0bdb-121">deviceUsageType</span><span class="sxs-lookup"><span data-stu-id="f0bdb-121">deviceUsageType</span></span>|[<span data-ttu-id="f0bdb-122">windowsDeviceUsageType</span><span class="sxs-lookup"><span data-stu-id="f0bdb-122">windowsDeviceUsageType</span></span>](../resources/intune-enrollment-windowsdeviceusagetype.md)|<span data-ttu-id="f0bdb-123">AAD 参加認証の種類。</span><span class="sxs-lookup"><span data-stu-id="f0bdb-123">AAD join authentication type.</span></span> <span data-ttu-id="f0bdb-124">使用可能な値は、`singleUser`、`shared` です。</span><span class="sxs-lookup"><span data-stu-id="f0bdb-124">Possible values are: `singleUser`, `shared`.</span></span>|
|<span data-ttu-id="f0bdb-125">skipキーボードの selectionpage</span><span class="sxs-lookup"><span data-stu-id="f0bdb-125">skipKeyboardSelectionPage</span></span>|<span data-ttu-id="f0bdb-126">ブール値</span><span class="sxs-lookup"><span data-stu-id="f0bdb-126">Boolean</span></span>|<span data-ttu-id="f0bdb-127">設定されている場合は、言語と地域が設定されている場合は、キーボードの選択ページをスキップします。</span><span class="sxs-lookup"><span data-stu-id="f0bdb-127">If set, then skip the keyboard selection page if Language and Region are set</span></span>|
|<span data-ttu-id="f0bdb-128">hideEscapeLink</span><span class="sxs-lookup"><span data-stu-id="f0bdb-128">hideEscapeLink</span></span>|<span data-ttu-id="f0bdb-129">ブール値</span><span class="sxs-lookup"><span data-stu-id="f0bdb-129">Boolean</span></span>|<span data-ttu-id="f0bdb-130">true に設定されている場合、ユーザーは別のアカウントを使用してサインインすることはできません (会社のサインイン時)。</span><span class="sxs-lookup"><span data-stu-id="f0bdb-130">If set to true, then the user can't start over with different account, on company sign-in</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0bdb-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f0bdb-131">Relationships</span></span>
<span data-ttu-id="f0bdb-132">なし</span><span class="sxs-lookup"><span data-stu-id="f0bdb-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f0bdb-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f0bdb-133">JSON Representation</span></span>
<span data-ttu-id="f0bdb-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f0bdb-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.outOfBoxExperienceSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.outOfBoxExperienceSettings",
  "hidePrivacySettings": true,
  "hideEULA": true,
  "userType": "String",
  "deviceUsageType": "String",
  "skipKeyboardSelectionPage": true,
  "hideEscapeLink": true
}
```




