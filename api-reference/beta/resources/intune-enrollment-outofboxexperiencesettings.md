---
title: outOfBoxExperienceSettings リソースの種類
description: ボックスの設定が発生します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5d2b48fef00c9c3a291a0a2fdfe680b9f4e21030
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404604"
---
# <a name="outofboxexperiencesettings-resource-type"></a><span data-ttu-id="e51f8-103">outOfBoxExperienceSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e51f8-103">outOfBoxExperienceSettings resource type</span></span>

> <span data-ttu-id="e51f8-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e51f8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e51f8-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e51f8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e51f8-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e51f8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e51f8-107">ボックスの設定が発生します。</span><span class="sxs-lookup"><span data-stu-id="e51f8-107">Out of box experience setting</span></span>

## <a name="properties"></a><span data-ttu-id="e51f8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e51f8-108">Properties</span></span>
|<span data-ttu-id="e51f8-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e51f8-109">Property</span></span>|<span data-ttu-id="e51f8-110">型</span><span class="sxs-lookup"><span data-stu-id="e51f8-110">Type</span></span>|<span data-ttu-id="e51f8-111">説明</span><span class="sxs-lookup"><span data-stu-id="e51f8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e51f8-112">hidePrivacySettings</span><span class="sxs-lookup"><span data-stu-id="e51f8-112">hidePrivacySettings</span></span>|<span data-ttu-id="e51f8-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51f8-113">Boolean</span></span>|<span data-ttu-id="e51f8-114">ユーザーのプライバシー設定の表示と非表示を切り替える</span><span class="sxs-lookup"><span data-stu-id="e51f8-114">Show or hide privacy settings to user</span></span>|
|<span data-ttu-id="e51f8-115">hideEULA</span><span class="sxs-lookup"><span data-stu-id="e51f8-115">hideEULA</span></span>|<span data-ttu-id="e51f8-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51f8-116">Boolean</span></span>|<span data-ttu-id="e51f8-117">ユーザーに使用許諾契約書の表示と非表示を切り替える</span><span class="sxs-lookup"><span data-stu-id="e51f8-117">Show or hide EULA to user</span></span>|
|<span data-ttu-id="e51f8-118">userType</span><span class="sxs-lookup"><span data-stu-id="e51f8-118">userType</span></span>|[<span data-ttu-id="e51f8-119">windowsUserType</span><span class="sxs-lookup"><span data-stu-id="e51f8-119">windowsUserType</span></span>](../resources/intune-enrollment-windowsusertype.md)|<span data-ttu-id="e51f8-120">ユーザーの種類です。</span><span class="sxs-lookup"><span data-stu-id="e51f8-120">Type of user.</span></span> <span data-ttu-id="e51f8-121">使用可能な値は、`administrator`、`standard` です。</span><span class="sxs-lookup"><span data-stu-id="e51f8-121">Possible values are: `administrator`, `standard`.</span></span>|
|<span data-ttu-id="e51f8-122">deviceUsageType</span><span class="sxs-lookup"><span data-stu-id="e51f8-122">deviceUsageType</span></span>|[<span data-ttu-id="e51f8-123">windowsDeviceUsageType</span><span class="sxs-lookup"><span data-stu-id="e51f8-123">windowsDeviceUsageType</span></span>](../resources/intune-enrollment-windowsdeviceusagetype.md)|<span data-ttu-id="e51f8-124">AAD の結合の認証の種類です。</span><span class="sxs-lookup"><span data-stu-id="e51f8-124">AAD join authentication type.</span></span> <span data-ttu-id="e51f8-125">使用可能な値は、`singleUser`、`shared` です。</span><span class="sxs-lookup"><span data-stu-id="e51f8-125">Possible values are: `singleUser`, `shared`.</span></span>|
|<span data-ttu-id="e51f8-126">skipKeyboardSelectionPage</span><span class="sxs-lookup"><span data-stu-id="e51f8-126">skipKeyboardSelectionPage</span></span>|<span data-ttu-id="e51f8-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51f8-127">Boolean</span></span>|<span data-ttu-id="e51f8-128">かどうか、セット、キーボードの選択をスキップするページの言語と地域が設定されている場合</span><span class="sxs-lookup"><span data-stu-id="e51f8-128">If set, then skip the keyboard selection page if Language and Region are set</span></span>|
|<span data-ttu-id="e51f8-129">hideEscapeLink</span><span class="sxs-lookup"><span data-stu-id="e51f8-129">hideEscapeLink</span></span>|<span data-ttu-id="e51f8-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51f8-130">Boolean</span></span>|<span data-ttu-id="e51f8-131">ユーザーでは、true に設定を別のアカウントでのサインインの会社経由で起動できない場合</span><span class="sxs-lookup"><span data-stu-id="e51f8-131">If set to true, then the user can't start over with different account, on company sign-in</span></span>|

## <a name="relationships"></a><span data-ttu-id="e51f8-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e51f8-132">Relationships</span></span>
<span data-ttu-id="e51f8-133">なし</span><span class="sxs-lookup"><span data-stu-id="e51f8-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e51f8-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e51f8-134">JSON Representation</span></span>
<span data-ttu-id="e51f8-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e51f8-135">Here is a JSON representation of the resource.</span></span>
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




