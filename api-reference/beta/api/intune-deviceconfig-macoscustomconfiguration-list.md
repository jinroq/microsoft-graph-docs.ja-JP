---
title: macOSCustomConfigurations のリスト
description: macOSCustomConfiguration オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
ms.openlocfilehash: 9c2783d5d6f8f8b2f88c98b322b5a53b5947e1d2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301758"
---
# <a name="list-macoscustomconfigurations"></a><span data-ttu-id="0f1d7-103">macOSCustomConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="0f1d7-103">List macOSCustomConfigurations</span></span>

> <span data-ttu-id="0f1d7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0f1d7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f1d7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0f1d7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0f1d7-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0f1d7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f1d7-107">[macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="0f1d7-107">List properties and relationships of the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0f1d7-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="0f1d7-108">Prerequisites</span></span>
<span data-ttu-id="0f1d7-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0f1d7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f1d7-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0f1d7-111">Permission type</span></span>|<span data-ttu-id="0f1d7-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0f1d7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f1d7-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0f1d7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0f1d7-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0f1d7-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0f1d7-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0f1d7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f1d7-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0f1d7-116">Not supported.</span></span>|
|<span data-ttu-id="0f1d7-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0f1d7-117">Application</span></span>|<span data-ttu-id="0f1d7-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0f1d7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f1d7-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0f1d7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0f1d7-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0f1d7-120">Request headers</span></span>
|<span data-ttu-id="0f1d7-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0f1d7-121">Header</span></span>|<span data-ttu-id="0f1d7-122">値</span><span class="sxs-lookup"><span data-stu-id="0f1d7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f1d7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f1d7-123">Authorization</span></span>|<span data-ttu-id="0f1d7-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="0f1d7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f1d7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0f1d7-125">Accept</span></span>|<span data-ttu-id="0f1d7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0f1d7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f1d7-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0f1d7-127">Request body</span></span>
<span data-ttu-id="0f1d7-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0f1d7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f1d7-129">応答</span><span class="sxs-lookup"><span data-stu-id="0f1d7-129">Response</span></span>
<span data-ttu-id="0f1d7-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="0f1d7-130">If successful, this method returns a `200 OK` response code and a collection of [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f1d7-131">例</span><span class="sxs-lookup"><span data-stu-id="0f1d7-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="0f1d7-132">要求</span><span class="sxs-lookup"><span data-stu-id="0f1d7-132">Request</span></span>
<span data-ttu-id="0f1d7-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0f1d7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="0f1d7-134">応答</span><span class="sxs-lookup"><span data-stu-id="0f1d7-134">Response</span></span>
<span data-ttu-id="0f1d7-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0f1d7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 634

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
      "id": "a253835d-835d-a253-5d83-53a25d8353a2",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "payloadName": "Payload Name value",
      "payloadFileName": "Payload File Name value",
      "payload": "cGF5bG9hZA=="
    }
  ]
}
```





