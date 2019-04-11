---
title: リスト deviceConfigurationConflictSummaries
description: deviceConfigurationConflictSummary オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 57c8ae67e0b09a289196c98d463ec68fe45c7a1f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776151"
---
# <a name="list-deviceconfigurationconflictsummaries"></a><span data-ttu-id="f1c01-103">リスト deviceConfigurationConflictSummaries</span><span class="sxs-lookup"><span data-stu-id="f1c01-103">List deviceConfigurationConflictSummaries</span></span>

> <span data-ttu-id="f1c01-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1c01-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1c01-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f1c01-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1c01-106">[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="f1c01-106">List properties and relationships of the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1c01-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f1c01-107">Prerequisites</span></span>
<span data-ttu-id="f1c01-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f1c01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1c01-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f1c01-110">Permission type</span></span>|<span data-ttu-id="f1c01-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f1c01-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1c01-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f1c01-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f1c01-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1c01-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f1c01-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f1c01-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1c01-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1c01-115">Not supported.</span></span>|
|<span data-ttu-id="f1c01-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f1c01-116">Application</span></span>|<span data-ttu-id="f1c01-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1c01-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1c01-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f1c01-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationConflictSummary
```

## <a name="request-headers"></a><span data-ttu-id="f1c01-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f1c01-119">Request headers</span></span>
|<span data-ttu-id="f1c01-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f1c01-120">Header</span></span>|<span data-ttu-id="f1c01-121">値</span><span class="sxs-lookup"><span data-stu-id="f1c01-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1c01-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1c01-122">Authorization</span></span>|<span data-ttu-id="f1c01-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f1c01-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1c01-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f1c01-124">Accept</span></span>|<span data-ttu-id="f1c01-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f1c01-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1c01-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f1c01-126">Request body</span></span>
<span data-ttu-id="f1c01-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f1c01-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1c01-128">応答</span><span class="sxs-lookup"><span data-stu-id="f1c01-128">Response</span></span>
<span data-ttu-id="f1c01-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="f1c01-129">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1c01-130">例</span><span class="sxs-lookup"><span data-stu-id="f1c01-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1c01-131">要求</span><span class="sxs-lookup"><span data-stu-id="f1c01-131">Request</span></span>
<span data-ttu-id="f1c01-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f1c01-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary
```

### <a name="response"></a><span data-ttu-id="f1c01-133">応答</span><span class="sxs-lookup"><span data-stu-id="f1c01-133">Response</span></span>
<span data-ttu-id="f1c01-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f1c01-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 495

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
      "conflictingDeviceConfigurations": [
        {
          "@odata.type": "microsoft.graph.settingSource",
          "id": "Id value",
          "displayName": "Display Name value"
        }
      ],
      "id": "d5f22c23-2c23-d5f2-232c-f2d5232cf2d5",
      "contributingSettings": [
        "Contributing Settings value"
      ],
      "deviceCheckinsImpacted": 6
    }
  ]
}
```





