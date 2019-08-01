---
title: reportRoot の更新
description: reportRoot オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 66448222ab82776a343296f6bec0be0e9d684852
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025828"
---
# <a name="update-reportroot"></a><span data-ttu-id="147af-103">reportRoot の更新</span><span class="sxs-lookup"><span data-stu-id="147af-103">Update reportRoot</span></span>

> <span data-ttu-id="147af-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="147af-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="147af-105">[reportRoot](../resources/intune-shared-reportroot.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="147af-105">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="147af-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="147af-106">Prerequisites</span></span>
<span data-ttu-id="147af-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="147af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="147af-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="147af-109">Permission type</span></span>|<span data-ttu-id="147af-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="147af-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="147af-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="147af-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="147af-112">&nbsp;&nbsp;デバイス構成</span><span class="sxs-lookup"><span data-stu-id="147af-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="147af-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="147af-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="147af-114">&nbsp;&nbsp;トラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="147af-114">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="147af-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="147af-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="147af-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="147af-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="147af-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="147af-117">Not supported.</span></span>|
|<span data-ttu-id="147af-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="147af-118">Application</span></span>|<span data-ttu-id="147af-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="147af-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="147af-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="147af-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="147af-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="147af-121">Request headers</span></span>
|<span data-ttu-id="147af-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="147af-122">Header</span></span>|<span data-ttu-id="147af-123">値</span><span class="sxs-lookup"><span data-stu-id="147af-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="147af-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="147af-124">Authorization</span></span>|<span data-ttu-id="147af-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="147af-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="147af-126">承諾</span><span class="sxs-lookup"><span data-stu-id="147af-126">Accept</span></span>|<span data-ttu-id="147af-127">application/json</span><span class="sxs-lookup"><span data-stu-id="147af-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="147af-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="147af-128">Request body</span></span>
<span data-ttu-id="147af-129">要求本文で、[reportRoot](../resources/intune-shared-reportroot.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="147af-129">In the request body, supply a JSON representation for the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

<span data-ttu-id="147af-130">次の表に、[reportRoot](../resources/intune-shared-reportroot.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="147af-130">The following table shows the properties that are required when you create the [reportRoot](../resources/intune-shared-reportroot.md).</span></span>

|<span data-ttu-id="147af-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="147af-131">Property</span></span>|<span data-ttu-id="147af-132">型</span><span class="sxs-lookup"><span data-stu-id="147af-132">Type</span></span>|<span data-ttu-id="147af-133">説明</span><span class="sxs-lookup"><span data-stu-id="147af-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="147af-134">id</span><span class="sxs-lookup"><span data-stu-id="147af-134">id</span></span>|<span data-ttu-id="147af-135">String</span><span class="sxs-lookup"><span data-stu-id="147af-135">String</span></span>|<span data-ttu-id="147af-136">このエンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="147af-136">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="147af-137">応答</span><span class="sxs-lookup"><span data-stu-id="147af-137">Response</span></span>
<span data-ttu-id="147af-138">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [reportRoot](../resources/intune-shared-reportroot.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="147af-138">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="147af-139">例</span><span class="sxs-lookup"><span data-stu-id="147af-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="147af-140">要求</span><span class="sxs-lookup"><span data-stu-id="147af-140">Request</span></span>
<span data-ttu-id="147af-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="147af-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/reports
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="147af-142">応答</span><span class="sxs-lookup"><span data-stu-id="147af-142">Response</span></span>
<span data-ttu-id="147af-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="147af-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```








