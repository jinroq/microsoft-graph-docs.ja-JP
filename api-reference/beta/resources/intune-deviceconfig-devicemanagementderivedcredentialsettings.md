---
title: deviceManagementDerivedCredentialSettings リソースの種類
description: 派生した資格情報のテナントレベルの設定を記述するエンティティ
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2fa7adfa76482cd4c67c2c3faaaf96b760f44bd2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33957061"
---
# <a name="devicemanagementderivedcredentialsettings-resource-type"></a><span data-ttu-id="d6f73-103">deviceManagementDerivedCredentialSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d6f73-103">deviceManagementDerivedCredentialSettings resource type</span></span>

> <span data-ttu-id="d6f73-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6f73-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6f73-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d6f73-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6f73-106">派生した資格情報のテナントレベルの設定を記述するエンティティ</span><span class="sxs-lookup"><span data-stu-id="d6f73-106">Entity that describes tenant level settings for derived credentials</span></span>

## <a name="methods"></a><span data-ttu-id="d6f73-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="d6f73-107">Methods</span></span>
|<span data-ttu-id="d6f73-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="d6f73-108">Method</span></span>|<span data-ttu-id="d6f73-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d6f73-109">Return Type</span></span>|<span data-ttu-id="d6f73-110">説明</span><span class="sxs-lookup"><span data-stu-id="d6f73-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d6f73-111">DeviceManagementDerivedCredentialSettings を取得する</span><span class="sxs-lookup"><span data-stu-id="d6f73-111">Get deviceManagementDerivedCredentialSettings</span></span>](../api/intune-deviceconfig-devicemanagementderivedcredentialsettings-get.md)|[<span data-ttu-id="d6f73-112">deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="d6f73-112">deviceManagementDerivedCredentialSettings</span></span>](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)|<span data-ttu-id="d6f73-113">[DeviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d6f73-113">Read properties and relationships of the [deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md) object.</span></span>|
|[<span data-ttu-id="d6f73-114">DeviceManagementDerivedCredentialSettings の更新</span><span class="sxs-lookup"><span data-stu-id="d6f73-114">Update deviceManagementDerivedCredentialSettings</span></span>](../api/intune-deviceconfig-devicemanagementderivedcredentialsettings-update.md)|[<span data-ttu-id="d6f73-115">deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="d6f73-115">deviceManagementDerivedCredentialSettings</span></span>](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)|<span data-ttu-id="d6f73-116">[DeviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d6f73-116">Update the properties of a [deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d6f73-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d6f73-117">Properties</span></span>
|<span data-ttu-id="d6f73-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d6f73-118">Property</span></span>|<span data-ttu-id="d6f73-119">型</span><span class="sxs-lookup"><span data-stu-id="d6f73-119">Type</span></span>|<span data-ttu-id="d6f73-120">説明</span><span class="sxs-lookup"><span data-stu-id="d6f73-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6f73-121">id</span><span class="sxs-lookup"><span data-stu-id="d6f73-121">id</span></span>|<span data-ttu-id="d6f73-122">文字列</span><span class="sxs-lookup"><span data-stu-id="d6f73-122">String</span></span>|<span data-ttu-id="d6f73-123">派生した資格情報の一意識別子</span><span class="sxs-lookup"><span data-stu-id="d6f73-123">Unique identifier for the Derived Credential</span></span>|
|<span data-ttu-id="d6f73-124">helpUrl</span><span class="sxs-lookup"><span data-stu-id="d6f73-124">helpUrl</span></span>|<span data-ttu-id="d6f73-125">String</span><span class="sxs-lookup"><span data-stu-id="d6f73-125">String</span></span>|<span data-ttu-id="d6f73-126">エンドユーザーが会社のポータルを使用して派生した資格情報を取得するときに、エンドユーザーがアクセスできる URL。</span><span class="sxs-lookup"><span data-stu-id="d6f73-126">The URL that will be accessible to end users as they retrieve a derived credential using the Company Portal.</span></span>|
|<span data-ttu-id="d6f73-127">displayName</span><span class="sxs-lookup"><span data-stu-id="d6f73-127">displayName</span></span>|<span data-ttu-id="d6f73-128">String</span><span class="sxs-lookup"><span data-stu-id="d6f73-128">String</span></span>|<span data-ttu-id="d6f73-129">プロファイルの表示名。</span><span class="sxs-lookup"><span data-stu-id="d6f73-129">The display name for the profile.</span></span>|
|<span data-ttu-id="d6f73-130">会社</span><span class="sxs-lookup"><span data-stu-id="d6f73-130">issuer</span></span>|[<span data-ttu-id="d6f73-131">deviceManagementDerivedCredentialIssuer</span><span class="sxs-lookup"><span data-stu-id="d6f73-131">deviceManagementDerivedCredentialIssuer</span></span>](../resources/intune-deviceconfig-devicemanagementderivedcredentialissuer.md)|<span data-ttu-id="d6f73-132">使用する派生資格情報プロバイダー。</span><span class="sxs-lookup"><span data-stu-id="d6f73-132">The derived credential provider to use.</span></span> <span data-ttu-id="d6f73-133">可能な値は、`intercede`、`entrustDatacard`、`purebred` です。</span><span class="sxs-lookup"><span data-stu-id="d6f73-133">Possible values are: `intercede`, `entrustDatacard`, `purebred`.</span></span>|
|<span data-ttu-id="d6f73-134">notificationType</span><span class="sxs-lookup"><span data-stu-id="d6f73-134">notificationType</span></span>|[<span data-ttu-id="d6f73-135">deviceManagementDerivedCredentialNotificationType</span><span class="sxs-lookup"><span data-stu-id="d6f73-135">deviceManagementDerivedCredentialNotificationType</span></span>](../resources/intune-deviceconfig-devicemanagementderivedcredentialnotificationtype.md)|<span data-ttu-id="d6f73-136">デバイスに証明書を使用する、Wi-fi、VPN、または電子メールプロファイルを配信するために、会社のポータルを開くことをエンドユーザーに通知するために使用されるメソッド。</span><span class="sxs-lookup"><span data-stu-id="d6f73-136">The methods used to inform the end user to open Company Portal to deliver Wi-Fi, VPN, or email profiles that use certificates to the device.</span></span> <span data-ttu-id="d6f73-137">可能な値は、`none`、`companyPortal`、`email` です。</span><span class="sxs-lookup"><span data-stu-id="d6f73-137">Possible values are: `none`, `companyPortal`, `email`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6f73-138">関係</span><span class="sxs-lookup"><span data-stu-id="d6f73-138">Relationships</span></span>
<span data-ttu-id="d6f73-139">なし</span><span class="sxs-lookup"><span data-stu-id="d6f73-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d6f73-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d6f73-140">JSON Representation</span></span>
<span data-ttu-id="d6f73-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d6f73-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementDerivedCredentialSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "id": "String (identifier)",
  "helpUrl": "String",
  "displayName": "String",
  "issuer": "String",
  "notificationType": "String"
}
```




