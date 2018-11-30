---
title: iosSingleSignOnSettings リソースの種類
description: iOS は単一のサインオンでの Kerberos 認証の設定
ms.openlocfilehash: a63848dc27afd037a6834a67c0736f86c06ac1fe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072958"
---
# <a name="iossinglesignonsettings-resource-type"></a><span data-ttu-id="b5d6d-103">iosSingleSignOnSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b5d6d-103">iosSingleSignOnSettings resource type</span></span>

> <span data-ttu-id="b5d6d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b5d6d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b5d6d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b5d6d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b5d6d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b5d6d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b5d6d-107">iOS は単一のサインオンでの Kerberos 認証の設定</span><span class="sxs-lookup"><span data-stu-id="b5d6d-107">iOS Kerberos authentication settings for single sign-on</span></span>
## <a name="properties"></a><span data-ttu-id="b5d6d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b5d6d-108">Properties</span></span>
|<span data-ttu-id="b5d6d-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b5d6d-109">Property</span></span>|<span data-ttu-id="b5d6d-110">型</span><span class="sxs-lookup"><span data-stu-id="b5d6d-110">Type</span></span>|<span data-ttu-id="b5d6d-111">説明</span><span class="sxs-lookup"><span data-stu-id="b5d6d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5d6d-112">allowedAppsList</span><span class="sxs-lookup"><span data-stu-id="b5d6d-112">allowedAppsList</span></span>|<span data-ttu-id="b5d6d-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b5d6d-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="b5d6d-114">このログインを使用するのには許可されているアプリケーションの識別子の一覧です。</span><span class="sxs-lookup"><span data-stu-id="b5d6d-114">List of app identifiers that are allowed to use this login.</span></span> <span data-ttu-id="b5d6d-115">このフィールドを省略すると、ログインは、デバイス上のすべてのアプリケーションに適用されます。</span><span class="sxs-lookup"><span data-stu-id="b5d6d-115">If this field is omitted, the login applies to all applications on the device.</span></span> <span data-ttu-id="b5d6d-116">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="b5d6d-116">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="b5d6d-117">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="b5d6d-117">allowedUrls</span></span>|<span data-ttu-id="b5d6d-118">String コレクション</span><span class="sxs-lookup"><span data-stu-id="b5d6d-118">String collection</span></span>|<span data-ttu-id="b5d6d-119">このログインを使用するために一致する必要がある HTTP Url の一覧です。</span><span class="sxs-lookup"><span data-stu-id="b5d6d-119">List of HTTP URLs that must be matched in order to use this login.</span></span> <span data-ttu-id="b5d6d-120">9.0 以降、iOS でワイルドカード文字を使用することがあります。</span><span class="sxs-lookup"><span data-stu-id="b5d6d-120">With iOS 9.0 or later, a wildcard characters may be used.</span></span>|
|<span data-ttu-id="b5d6d-121">displayName</span><span class="sxs-lookup"><span data-stu-id="b5d6d-121">displayName</span></span>|<span data-ttu-id="b5d6d-122">String</span><span class="sxs-lookup"><span data-stu-id="b5d6d-122">String</span></span>|<span data-ttu-id="b5d6d-123">受信側デバイスに表示されるログインの設定の表示名。</span><span class="sxs-lookup"><span data-stu-id="b5d6d-123">The display name of login settings shown on the receiving device.</span></span>|
|<span data-ttu-id="b5d6d-124">kerberosPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b5d6d-124">kerberosPrincipalName</span></span>|<span data-ttu-id="b5d6d-125">String</span><span class="sxs-lookup"><span data-stu-id="b5d6d-125">String</span></span>|<span data-ttu-id="b5d6d-126">Kerberos プリンシパルの名前です。</span><span class="sxs-lookup"><span data-stu-id="b5d6d-126">A Kerberos principal name.</span></span> <span data-ttu-id="b5d6d-127">指定しない場合、プロファイルのインストール時にいずれかの入力が求められます。</span><span class="sxs-lookup"><span data-stu-id="b5d6d-127">If not provided, the user is prompted for one during profile installation.</span></span>|
|<span data-ttu-id="b5d6d-128">kerberosRealm</span><span class="sxs-lookup"><span data-stu-id="b5d6d-128">kerberosRealm</span></span>|<span data-ttu-id="b5d6d-129">String</span><span class="sxs-lookup"><span data-stu-id="b5d6d-129">String</span></span>|<span data-ttu-id="b5d6d-130">Kerberos レルムの名前です。</span><span class="sxs-lookup"><span data-stu-id="b5d6d-130">A Kerberos realm name.</span></span> <span data-ttu-id="b5d6d-131">大文字小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="b5d6d-131">Case sensitive.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5d6d-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b5d6d-132">Relationships</span></span>
<span data-ttu-id="b5d6d-133">なし</span><span class="sxs-lookup"><span data-stu-id="b5d6d-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b5d6d-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b5d6d-134">JSON Representation</span></span>
<span data-ttu-id="b5d6d-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b5d6d-135">Here is a JSON representation of the resource.</span></span>
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





