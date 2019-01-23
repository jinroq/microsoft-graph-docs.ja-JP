---
title: reportRoot の更新
description: reportRoot オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3127ca7804883c5e29fe91cf5e21bb15240a1314
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422489"
---
# <a name="update-reportroot"></a><span data-ttu-id="b8339-103">reportRoot の更新</span><span class="sxs-lookup"><span data-stu-id="b8339-103">Update reportRoot</span></span>

> <span data-ttu-id="b8339-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b8339-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b8339-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b8339-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b8339-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b8339-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8339-107">[reportRoot](../resources/intune-shared-reportroot.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b8339-107">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b8339-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="b8339-108">Prerequisites</span></span>
<span data-ttu-id="b8339-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b8339-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8339-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b8339-111">Permission type</span></span>|<span data-ttu-id="b8339-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b8339-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8339-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b8339-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b8339-114">&nbsp; &nbsp; **デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="b8339-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="b8339-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8339-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="b8339-116">&nbsp; &nbsp; **トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="b8339-116">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="b8339-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8339-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b8339-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b8339-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8339-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b8339-119">Not supported.</span></span>|
|<span data-ttu-id="b8339-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b8339-120">Application</span></span>|<span data-ttu-id="b8339-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b8339-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8339-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b8339-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="b8339-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b8339-123">Request headers</span></span>
|<span data-ttu-id="b8339-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b8339-124">Header</span></span>|<span data-ttu-id="b8339-125">値</span><span class="sxs-lookup"><span data-stu-id="b8339-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8339-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8339-126">Authorization</span></span>|<span data-ttu-id="b8339-127">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b8339-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8339-128">Accept</span><span class="sxs-lookup"><span data-stu-id="b8339-128">Accept</span></span>|<span data-ttu-id="b8339-129">application/json</span><span class="sxs-lookup"><span data-stu-id="b8339-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8339-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="b8339-130">Request body</span></span>
<span data-ttu-id="b8339-131">要求本文で、[reportRoot](../resources/intune-shared-reportroot.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b8339-131">In the request body, supply a JSON representation for the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

<span data-ttu-id="b8339-132">次の表に、[reportRoot](../resources/intune-shared-reportroot.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b8339-132">The following table shows the properties that are required when you create the [reportRoot](../resources/intune-shared-reportroot.md).</span></span>

|<span data-ttu-id="b8339-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8339-133">Property</span></span>|<span data-ttu-id="b8339-134">型</span><span class="sxs-lookup"><span data-stu-id="b8339-134">Type</span></span>|<span data-ttu-id="b8339-135">説明</span><span class="sxs-lookup"><span data-stu-id="b8339-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8339-136">id</span><span class="sxs-lookup"><span data-stu-id="b8339-136">id</span></span>|<span data-ttu-id="b8339-137">String</span><span class="sxs-lookup"><span data-stu-id="b8339-137">String</span></span>|<span data-ttu-id="b8339-138">このエンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="b8339-138">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="b8339-139">応答</span><span class="sxs-lookup"><span data-stu-id="b8339-139">Response</span></span>
<span data-ttu-id="b8339-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [reportRoot](../resources/intune-shared-reportroot.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b8339-140">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8339-141">例</span><span class="sxs-lookup"><span data-stu-id="b8339-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="b8339-142">要求</span><span class="sxs-lookup"><span data-stu-id="b8339-142">Request</span></span>
<span data-ttu-id="b8339-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b8339-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/reports
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="b8339-144">応答</span><span class="sxs-lookup"><span data-stu-id="b8339-144">Response</span></span>
<span data-ttu-id="b8339-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b8339-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```



