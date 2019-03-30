---
title: リスト androidforwork custom構成
description: androidforwork customconfiguration オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4183265ae2f8addf0f9e609b3bbafd8bd912ee7f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30965173"
---
# <a name="list-androidforworkcustomconfigurations"></a><span data-ttu-id="638cb-103">リスト androidforwork custom構成</span><span class="sxs-lookup"><span data-stu-id="638cb-103">List androidForWorkCustomConfigurations</span></span>

> <span data-ttu-id="638cb-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="638cb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="638cb-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="638cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="638cb-106">[androidforwork customconfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="638cb-106">List properties and relationships of the [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="638cb-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="638cb-107">Prerequisites</span></span>
<span data-ttu-id="638cb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="638cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="638cb-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="638cb-110">Permission type</span></span>|<span data-ttu-id="638cb-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="638cb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="638cb-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="638cb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="638cb-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="638cb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="638cb-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="638cb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="638cb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="638cb-115">Not supported.</span></span>|
|<span data-ttu-id="638cb-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="638cb-116">Application</span></span>|<span data-ttu-id="638cb-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="638cb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="638cb-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="638cb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="638cb-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="638cb-119">Request headers</span></span>
|<span data-ttu-id="638cb-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="638cb-120">Header</span></span>|<span data-ttu-id="638cb-121">値</span><span class="sxs-lookup"><span data-stu-id="638cb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="638cb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="638cb-122">Authorization</span></span>|<span data-ttu-id="638cb-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="638cb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="638cb-124">承諾</span><span class="sxs-lookup"><span data-stu-id="638cb-124">Accept</span></span>|<span data-ttu-id="638cb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="638cb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="638cb-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="638cb-126">Request body</span></span>
<span data-ttu-id="638cb-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="638cb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="638cb-128">応答</span><span class="sxs-lookup"><span data-stu-id="638cb-128">Response</span></span>
<span data-ttu-id="638cb-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[androidforwork customconfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="638cb-129">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="638cb-130">例</span><span class="sxs-lookup"><span data-stu-id="638cb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="638cb-131">要求</span><span class="sxs-lookup"><span data-stu-id="638cb-131">Request</span></span>
<span data-ttu-id="638cb-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="638cb-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="638cb-133">応答</span><span class="sxs-lookup"><span data-stu-id="638cb-133">Response</span></span>
<span data-ttu-id="638cb-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="638cb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 786

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkCustomConfiguration",
      "id": "cca8b2bb-b2bb-cca8-bbb2-a8ccbbb2a8cc",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "omaSettings": [
        {
          "@odata.type": "microsoft.graph.omaSettingInteger",
          "displayName": "Display Name value",
          "description": "Description value",
          "omaUri": "Oma Uri value",
          "value": 5
        }
      ]
    }
  ]
}
```




