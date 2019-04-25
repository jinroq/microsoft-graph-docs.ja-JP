---
title: onPremisesConditionalAccessSettings リソースの種類
description: テナントの Exchange OnPremises 条件付きアクセス設定を表す単一エンティティ。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8fe4dd79722392ea5c0e5e6487c3c3dbc3587d4e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566452"
---
# <a name="onpremisesconditionalaccesssettings-resource-type"></a><span data-ttu-id="546e9-103">onPremisesConditionalAccessSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="546e9-103">onPremisesConditionalAccessSettings resource type</span></span>

> <span data-ttu-id="546e9-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="546e9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="546e9-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="546e9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="546e9-106">テナントの Exchange OnPremises 条件付きアクセス設定を表す単一エンティティ。</span><span class="sxs-lookup"><span data-stu-id="546e9-106">Singleton entity which represents the Exchange OnPremises Conditional Access Settings for a tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="546e9-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="546e9-107">Methods</span></span>
|<span data-ttu-id="546e9-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="546e9-108">Method</span></span>|<span data-ttu-id="546e9-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="546e9-109">Return Type</span></span>|<span data-ttu-id="546e9-110">説明</span><span class="sxs-lookup"><span data-stu-id="546e9-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="546e9-111">Get onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="546e9-111">Get onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-get.md)|[<span data-ttu-id="546e9-112">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="546e9-112">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="546e9-113">[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="546e9-113">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|
|[<span data-ttu-id="546e9-114">Update onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="546e9-114">Update onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-update.md)|[<span data-ttu-id="546e9-115">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="546e9-115">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="546e9-116">[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="546e9-116">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="546e9-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="546e9-117">Properties</span></span>
|<span data-ttu-id="546e9-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="546e9-118">Property</span></span>|<span data-ttu-id="546e9-119">型</span><span class="sxs-lookup"><span data-stu-id="546e9-119">Type</span></span>|<span data-ttu-id="546e9-120">説明</span><span class="sxs-lookup"><span data-stu-id="546e9-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="546e9-121">id</span><span class="sxs-lookup"><span data-stu-id="546e9-121">id</span></span>|<span data-ttu-id="546e9-122">String</span><span class="sxs-lookup"><span data-stu-id="546e9-122">String</span></span>|<span data-ttu-id="546e9-123">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="546e9-123">Not yet documented</span></span>|
|<span data-ttu-id="546e9-124">enabled</span><span class="sxs-lookup"><span data-stu-id="546e9-124">enabled</span></span>|<span data-ttu-id="546e9-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="546e9-125">Boolean</span></span>|<span data-ttu-id="546e9-126">対象組織で、オンプレミスの条件付きアクセスが有効かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="546e9-126">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="546e9-127">includedGroups</span><span class="sxs-lookup"><span data-stu-id="546e9-127">includedGroups</span></span>|<span data-ttu-id="546e9-128">Guid コレクション</span><span class="sxs-lookup"><span data-stu-id="546e9-128">Guid collection</span></span>|<span data-ttu-id="546e9-129">オンプレミスの条件付きアクセスで対象となるユーザー グループ。</span><span class="sxs-lookup"><span data-stu-id="546e9-129">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="546e9-130">これらのグループ内のユーザーすべては、管理対象のモバイル デバイスを持っており、メール アクセスに準拠している必要があります。</span><span class="sxs-lookup"><span data-stu-id="546e9-130">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="546e9-131">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="546e9-131">excludedGroups</span></span>|<span data-ttu-id="546e9-132">Guid コレクション</span><span class="sxs-lookup"><span data-stu-id="546e9-132">Guid collection</span></span>|<span data-ttu-id="546e9-133">オンプレミスの条件付きアクセスで除外されるユーザー グループ。</span><span class="sxs-lookup"><span data-stu-id="546e9-133">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="546e9-134">これらのグループ内のすべてのユーザーは、条件付きアクセス ポリシーから除外されます。</span><span class="sxs-lookup"><span data-stu-id="546e9-134">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="546e9-135">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="546e9-135">overrideDefaultRule</span></span>|<span data-ttu-id="546e9-136">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="546e9-136">Boolean</span></span>|<span data-ttu-id="546e9-137">デバイスでアクセスが付与されていることを確認できるようにするとき、既定のアクセス ルールを上書きします。</span><span class="sxs-lookup"><span data-stu-id="546e9-137">Override the default access rule when allowing a device to ensure access is granted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="546e9-138">関係</span><span class="sxs-lookup"><span data-stu-id="546e9-138">Relationships</span></span>
<span data-ttu-id="546e9-139">なし</span><span class="sxs-lookup"><span data-stu-id="546e9-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="546e9-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="546e9-140">JSON Representation</span></span>
<span data-ttu-id="546e9-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="546e9-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onPremisesConditionalAccessSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "String (identifier)",
  "enabled": true,
  "includedGroups": [
    "Guid"
  ],
  "excludedGroups": [
    "Guid"
  ],
  "overrideDefaultRule": true
}
```





