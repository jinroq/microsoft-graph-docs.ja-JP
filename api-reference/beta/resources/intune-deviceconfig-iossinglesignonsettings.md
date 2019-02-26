---
title: iosSingleSignOnSettings リソースの種類
description: シングルサインオンの iOS Kerberos 認証設定
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7b438ea8fadc30a0bf5fa3786e9b4cec3344093c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142624"
---
# <a name="iossinglesignonsettings-resource-type"></a><span data-ttu-id="135fb-103">iosSingleSignOnSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="135fb-103">iosSingleSignOnSettings resource type</span></span>

> <span data-ttu-id="135fb-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="135fb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="135fb-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="135fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="135fb-106">シングルサインオンの iOS Kerberos 認証設定</span><span class="sxs-lookup"><span data-stu-id="135fb-106">iOS Kerberos authentication settings for single sign-on</span></span>

## <a name="properties"></a><span data-ttu-id="135fb-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="135fb-107">Properties</span></span>
|<span data-ttu-id="135fb-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="135fb-108">Property</span></span>|<span data-ttu-id="135fb-109">型</span><span class="sxs-lookup"><span data-stu-id="135fb-109">Type</span></span>|<span data-ttu-id="135fb-110">説明</span><span class="sxs-lookup"><span data-stu-id="135fb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="135fb-111">allowedappslist プロパティ</span><span class="sxs-lookup"><span data-stu-id="135fb-111">allowedAppsList</span></span>|<span data-ttu-id="135fb-112">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="135fb-112">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="135fb-113">このログインの使用が許可されているアプリ識別子のリスト。</span><span class="sxs-lookup"><span data-stu-id="135fb-113">List of app identifiers that are allowed to use this login.</span></span> <span data-ttu-id="135fb-114">このフィールドを省略した場合、ログインはデバイス上のすべてのアプリケーションに適用されます。</span><span class="sxs-lookup"><span data-stu-id="135fb-114">If this field is omitted, the login applies to all applications on the device.</span></span> <span data-ttu-id="135fb-115">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="135fb-115">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="135fb-116">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="135fb-116">allowedUrls</span></span>|<span data-ttu-id="135fb-117">String コレクション</span><span class="sxs-lookup"><span data-stu-id="135fb-117">String collection</span></span>|<span data-ttu-id="135fb-118">このログインを使用するために一致する必要がある HTTP url のリスト。</span><span class="sxs-lookup"><span data-stu-id="135fb-118">List of HTTP URLs that must be matched in order to use this login.</span></span> <span data-ttu-id="135fb-119">iOS 9.0 以降では、ワイルドカード文字を使用することができます。</span><span class="sxs-lookup"><span data-stu-id="135fb-119">With iOS 9.0 or later, a wildcard characters may be used.</span></span>|
|<span data-ttu-id="135fb-120">displayName</span><span class="sxs-lookup"><span data-stu-id="135fb-120">displayName</span></span>|<span data-ttu-id="135fb-121">String</span><span class="sxs-lookup"><span data-stu-id="135fb-121">String</span></span>|<span data-ttu-id="135fb-122">受信側デバイスに表示されるログイン設定の表示名。</span><span class="sxs-lookup"><span data-stu-id="135fb-122">The display name of login settings shown on the receiving device.</span></span>|
|<span data-ttu-id="135fb-123">kerberosPrincipalName</span><span class="sxs-lookup"><span data-stu-id="135fb-123">kerberosPrincipalName</span></span>|<span data-ttu-id="135fb-124">String</span><span class="sxs-lookup"><span data-stu-id="135fb-124">String</span></span>|<span data-ttu-id="135fb-125">Kerberos プリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="135fb-125">A Kerberos principal name.</span></span> <span data-ttu-id="135fb-126">指定しない場合、プロファイルのインストール時にユーザーに対してプロンプトが表示されます。</span><span class="sxs-lookup"><span data-stu-id="135fb-126">If not provided, the user is prompted for one during profile installation.</span></span>|
|<span data-ttu-id="135fb-127">kerberosRealm</span><span class="sxs-lookup"><span data-stu-id="135fb-127">kerberosRealm</span></span>|<span data-ttu-id="135fb-128">String</span><span class="sxs-lookup"><span data-stu-id="135fb-128">String</span></span>|<span data-ttu-id="135fb-129">Kerberos 領域名。</span><span class="sxs-lookup"><span data-stu-id="135fb-129">A Kerberos realm name.</span></span> <span data-ttu-id="135fb-130">大文字小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="135fb-130">Case sensitive.</span></span>|

## <a name="relationships"></a><span data-ttu-id="135fb-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="135fb-131">Relationships</span></span>
<span data-ttu-id="135fb-132">なし</span><span class="sxs-lookup"><span data-stu-id="135fb-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="135fb-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="135fb-133">JSON Representation</span></span>
<span data-ttu-id="135fb-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="135fb-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosSingleSignOnSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosSingleSignOnSettings",
  "allowedAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "allowedUrls": [
    "String"
  ],
  "displayName": "String",
  "kerberosPrincipalName": "String",
  "kerberosRealm": "String"
}
```




