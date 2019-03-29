---
title: windowsdomainjoinconfigurations を一覧表示する
description: windowsdomainjoinconfiguration オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 19f4687039e2a07b32994d855f3e215da2af85c8
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30960266"
---
# <a name="list-windowsdomainjoinconfigurations"></a><span data-ttu-id="e5b06-103">windowsdomainjoinconfigurations を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e5b06-103">List windowsDomainJoinConfigurations</span></span>

> <span data-ttu-id="e5b06-104">**重要:** Microsoft Graph の/ベータ版の api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="e5b06-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e5b06-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5b06-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e5b06-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e5b06-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5b06-107">[windowsdomainjoinconfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="e5b06-107">List properties and relationships of the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e5b06-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="e5b06-108">Prerequisites</span></span>
<span data-ttu-id="e5b06-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e5b06-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5b06-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e5b06-111">Permission type</span></span>|<span data-ttu-id="e5b06-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e5b06-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5b06-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e5b06-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e5b06-114">&nbsp; &nbsp; **デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="e5b06-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="e5b06-115">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e5b06-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e5b06-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e5b06-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5b06-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5b06-117">Not supported.</span></span>|
|<span data-ttu-id="e5b06-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e5b06-118">Application</span></span>|<span data-ttu-id="e5b06-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5b06-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5b06-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e5b06-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e5b06-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e5b06-121">Request headers</span></span>
|<span data-ttu-id="e5b06-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e5b06-122">Header</span></span>|<span data-ttu-id="e5b06-123">値</span><span class="sxs-lookup"><span data-stu-id="e5b06-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5b06-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5b06-124">Authorization</span></span>|<span data-ttu-id="e5b06-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e5b06-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5b06-126">承諾</span><span class="sxs-lookup"><span data-stu-id="e5b06-126">Accept</span></span>|<span data-ttu-id="e5b06-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e5b06-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5b06-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="e5b06-128">Request body</span></span>
<span data-ttu-id="e5b06-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e5b06-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5b06-130">応答</span><span class="sxs-lookup"><span data-stu-id="e5b06-130">Response</span></span>
<span data-ttu-id="e5b06-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[windowsdomainjoinconfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e5b06-131">If successful, this method returns a `200 OK` response code and a collection of [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5b06-132">例</span><span class="sxs-lookup"><span data-stu-id="e5b06-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="e5b06-133">要求</span><span class="sxs-lookup"><span data-stu-id="e5b06-133">Request</span></span>
<span data-ttu-id="e5b06-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e5b06-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="e5b06-135">応答</span><span class="sxs-lookup"><span data-stu-id="e5b06-135">Response</span></span>
<span data-ttu-id="e5b06-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e5b06-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 760

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsDomainJoinConfiguration",
      "id": "40118d08-8d08-4011-088d-1140088d1140",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "computerNameStaticPrefix": "Computer Name Static Prefix value",
      "computerNameSuffixRandomCharCount": 1,
      "activeDirectoryDomainName": "Active Directory Domain Name value",
      "organizationalUnit": "Organizational Unit value"
    }
  ]
}
```



