---
title: deviceManagementDerivedCredentialSettings リソースの種類
description: 派生した資格情報のテナントレベルの設定を記述するエンティティ
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c2b9d81cf542681bc2ef610ebe86e836d7c84412
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332779"
---
# <a name="devicemanagementderivedcredentialsettings-resource-type"></a><span data-ttu-id="0f51f-103">deviceManagementDerivedCredentialSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0f51f-103">deviceManagementDerivedCredentialSettings resource type</span></span>

> <span data-ttu-id="0f51f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0f51f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f51f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0f51f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f51f-106">派生した資格情報のテナントレベルの設定を記述するエンティティ</span><span class="sxs-lookup"><span data-stu-id="0f51f-106">Entity that describes tenant level settings for derived credentials</span></span>

## <a name="methods"></a><span data-ttu-id="0f51f-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="0f51f-107">Methods</span></span>
|<span data-ttu-id="0f51f-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="0f51f-108">Method</span></span>|<span data-ttu-id="0f51f-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0f51f-109">Return Type</span></span>|<span data-ttu-id="0f51f-110">説明</span><span class="sxs-lookup"><span data-stu-id="0f51f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0f51f-111">DeviceManagementDerivedCredentialSettings を取得する</span><span class="sxs-lookup"><span data-stu-id="0f51f-111">Get deviceManagementDerivedCredentialSettings</span></span>](../api/intune-deviceconfig-devicemanagementderivedcredentialsettings-get.md)|[<span data-ttu-id="0f51f-112">deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="0f51f-112">deviceManagementDerivedCredentialSettings</span></span>](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)|<span data-ttu-id="0f51f-113">[DeviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0f51f-113">Read properties and relationships of the [deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md) object.</span></span>|
|[<span data-ttu-id="0f51f-114">DeviceManagementDerivedCredentialSettings の更新</span><span class="sxs-lookup"><span data-stu-id="0f51f-114">Update deviceManagementDerivedCredentialSettings</span></span>](../api/intune-deviceconfig-devicemanagementderivedcredentialsettings-update.md)|[<span data-ttu-id="0f51f-115">deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="0f51f-115">deviceManagementDerivedCredentialSettings</span></span>](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)|<span data-ttu-id="0f51f-116">[DeviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0f51f-116">Update the properties of a [deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0f51f-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0f51f-117">Properties</span></span>
|<span data-ttu-id="0f51f-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0f51f-118">Property</span></span>|<span data-ttu-id="0f51f-119">型</span><span class="sxs-lookup"><span data-stu-id="0f51f-119">Type</span></span>|<span data-ttu-id="0f51f-120">説明</span><span class="sxs-lookup"><span data-stu-id="0f51f-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f51f-121">id</span><span class="sxs-lookup"><span data-stu-id="0f51f-121">id</span></span>|<span data-ttu-id="0f51f-122">文字列</span><span class="sxs-lookup"><span data-stu-id="0f51f-122">String</span></span>|<span data-ttu-id="0f51f-123">派生した資格情報の一意識別子</span><span class="sxs-lookup"><span data-stu-id="0f51f-123">Unique identifier for the Derived Credential</span></span>|
|<span data-ttu-id="0f51f-124">helpUrl</span><span class="sxs-lookup"><span data-stu-id="0f51f-124">helpUrl</span></span>|<span data-ttu-id="0f51f-125">String</span><span class="sxs-lookup"><span data-stu-id="0f51f-125">String</span></span>|<span data-ttu-id="0f51f-126">エンドユーザーが会社のポータルを使用して派生した資格情報を取得するときに、エンドユーザーがアクセスできる URL。</span><span class="sxs-lookup"><span data-stu-id="0f51f-126">The URL that will be accessible to end users as they retrieve a derived credential using the Company Portal.</span></span>|
|<span data-ttu-id="0f51f-127">displayName</span><span class="sxs-lookup"><span data-stu-id="0f51f-127">displayName</span></span>|<span data-ttu-id="0f51f-128">String</span><span class="sxs-lookup"><span data-stu-id="0f51f-128">String</span></span>|<span data-ttu-id="0f51f-129">プロファイルの表示名。</span><span class="sxs-lookup"><span data-stu-id="0f51f-129">The display name for the profile.</span></span>|
|<span data-ttu-id="0f51f-130">会社</span><span class="sxs-lookup"><span data-stu-id="0f51f-130">issuer</span></span>|[<span data-ttu-id="0f51f-131">deviceManagementDerivedCredentialIssuer</span><span class="sxs-lookup"><span data-stu-id="0f51f-131">deviceManagementDerivedCredentialIssuer</span></span>](../resources/intune-deviceconfig-devicemanagementderivedcredentialissuer.md)|<span data-ttu-id="0f51f-132">使用する派生資格情報プロバイダー。</span><span class="sxs-lookup"><span data-stu-id="0f51f-132">The derived credential provider to use.</span></span> <span data-ttu-id="0f51f-133">可能な値は、`intercede`、`entrustDatacard`、`purebred` です。</span><span class="sxs-lookup"><span data-stu-id="0f51f-133">Possible values are: `intercede`, `entrustDatacard`, `purebred`.</span></span>|
|<span data-ttu-id="0f51f-134">notificationType</span><span class="sxs-lookup"><span data-stu-id="0f51f-134">notificationType</span></span>|[<span data-ttu-id="0f51f-135">deviceManagementDerivedCredentialNotificationType</span><span class="sxs-lookup"><span data-stu-id="0f51f-135">deviceManagementDerivedCredentialNotificationType</span></span>](../resources/intune-deviceconfig-devicemanagementderivedcredentialnotificationtype.md)|<span data-ttu-id="0f51f-136">デバイスに証明書を使用する、Wi-fi、VPN、または電子メールプロファイルを配信するために、会社のポータルを開くことをエンドユーザーに通知するために使用されるメソッド。</span><span class="sxs-lookup"><span data-stu-id="0f51f-136">The methods used to inform the end user to open Company Portal to deliver Wi-Fi, VPN, or email profiles that use certificates to the device.</span></span> <span data-ttu-id="0f51f-137">可能な値は、`none`、`companyPortal`、`email` です。</span><span class="sxs-lookup"><span data-stu-id="0f51f-137">Possible values are: `none`, `companyPortal`, `email`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f51f-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0f51f-138">Relationships</span></span>
<span data-ttu-id="0f51f-139">なし</span><span class="sxs-lookup"><span data-stu-id="0f51f-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f51f-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0f51f-140">JSON Representation</span></span>
<span data-ttu-id="0f51f-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0f51f-141">Here is a JSON representation of the resource.</span></span>
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



