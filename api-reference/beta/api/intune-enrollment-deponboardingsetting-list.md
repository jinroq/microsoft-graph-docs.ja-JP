---
title: depon掲示板の設定を一覧表示する
description: deponboardingsetting オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9c8ffd4ac7b76a692978c73362ec94400facf139
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141462"
---
# <a name="list-deponboardingsettings"></a><span data-ttu-id="2edcb-103">depon掲示板の設定を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="2edcb-103">List depOnboardingSettings</span></span>

> <span data-ttu-id="2edcb-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2edcb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2edcb-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2edcb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2edcb-106">[deponboardingsetting](../resources/intune-enrollment-deponboardingsetting.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="2edcb-106">List properties and relationships of the [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2edcb-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="2edcb-107">Prerequisites</span></span>
<span data-ttu-id="2edcb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2edcb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2edcb-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2edcb-110">Permission type</span></span>|<span data-ttu-id="2edcb-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2edcb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2edcb-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2edcb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2edcb-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2edcb-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2edcb-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2edcb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2edcb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2edcb-115">Not supported.</span></span>|
|<span data-ttu-id="2edcb-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2edcb-116">Application</span></span>|<span data-ttu-id="2edcb-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2edcb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2edcb-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2edcb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings
```

## <a name="request-headers"></a><span data-ttu-id="2edcb-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2edcb-119">Request headers</span></span>
|<span data-ttu-id="2edcb-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2edcb-120">Header</span></span>|<span data-ttu-id="2edcb-121">値</span><span class="sxs-lookup"><span data-stu-id="2edcb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2edcb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2edcb-122">Authorization</span></span>|<span data-ttu-id="2edcb-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="2edcb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2edcb-124">承諾</span><span class="sxs-lookup"><span data-stu-id="2edcb-124">Accept</span></span>|<span data-ttu-id="2edcb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2edcb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2edcb-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="2edcb-126">Request body</span></span>
<span data-ttu-id="2edcb-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2edcb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2edcb-128">応答</span><span class="sxs-lookup"><span data-stu-id="2edcb-128">Response</span></span>
<span data-ttu-id="2edcb-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[depon掲示設定](../resources/intune-enrollment-deponboardingsetting.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="2edcb-129">If successful, this method returns a `200 OK` response code and a collection of [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2edcb-130">例</span><span class="sxs-lookup"><span data-stu-id="2edcb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2edcb-131">要求</span><span class="sxs-lookup"><span data-stu-id="2edcb-131">Request</span></span>
<span data-ttu-id="2edcb-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2edcb-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings
```

### <a name="response"></a><span data-ttu-id="2edcb-133">応答</span><span class="sxs-lookup"><span data-stu-id="2edcb-133">Response</span></span>
<span data-ttu-id="2edcb-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2edcb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 786

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.depOnboardingSetting",
      "id": "40342229-2229-4034-2922-344029223440",
      "appleIdentifier": "Apple Identifier value",
      "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "lastSuccessfulSyncDateTime": "2017-01-01T00:03:28.120883-08:00",
      "lastSyncTriggeredDateTime": "2017-01-01T00:00:02.0916369-08:00",
      "shareTokenWithSchoolDataSyncService": true,
      "lastSyncErrorCode": 1,
      "tokenType": "dep",
      "tokenName": "Token Name value",
      "syncedDeviceCount": 1,
      "dataSharingConsentGranted": true,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```




