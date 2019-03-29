---
title: windows10CustomConfigurations のリスト
description: windows10CustomConfiguration オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 395030c74bb1b4a9cbdb1588d7b4a9765942baba
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962989"
---
# <a name="list-windows10customconfigurations"></a><span data-ttu-id="87058-103">windows10CustomConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="87058-103">List windows10CustomConfigurations</span></span>

> <span data-ttu-id="87058-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="87058-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87058-105">[windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="87058-105">List properties and relationships of the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87058-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="87058-106">Prerequisites</span></span>
<span data-ttu-id="87058-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="87058-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87058-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="87058-109">Permission type</span></span>|<span data-ttu-id="87058-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="87058-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87058-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="87058-111">Delegated (work or school account)</span></span>|<span data-ttu-id="87058-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="87058-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="87058-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="87058-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87058-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="87058-114">Not supported.</span></span>|
|<span data-ttu-id="87058-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="87058-115">Application</span></span>|<span data-ttu-id="87058-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="87058-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87058-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="87058-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="87058-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="87058-118">Request headers</span></span>
|<span data-ttu-id="87058-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="87058-119">Header</span></span>|<span data-ttu-id="87058-120">値</span><span class="sxs-lookup"><span data-stu-id="87058-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87058-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="87058-121">Authorization</span></span>|<span data-ttu-id="87058-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="87058-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87058-123">承諾</span><span class="sxs-lookup"><span data-stu-id="87058-123">Accept</span></span>|<span data-ttu-id="87058-124">application/json</span><span class="sxs-lookup"><span data-stu-id="87058-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87058-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="87058-125">Request body</span></span>
<span data-ttu-id="87058-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="87058-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87058-127">応答</span><span class="sxs-lookup"><span data-stu-id="87058-127">Response</span></span>
<span data-ttu-id="87058-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="87058-128">If successful, this method returns a `200 OK` response code and a collection of [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87058-129">例</span><span class="sxs-lookup"><span data-stu-id="87058-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="87058-130">要求</span><span class="sxs-lookup"><span data-stu-id="87058-130">Request</span></span>
<span data-ttu-id="87058-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="87058-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="87058-132">応答</span><span class="sxs-lookup"><span data-stu-id="87058-132">Response</span></span>
<span data-ttu-id="87058-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="87058-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 673

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
      "id": "d8ae266e-266e-d8ae-6e26-aed86e26aed8",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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



