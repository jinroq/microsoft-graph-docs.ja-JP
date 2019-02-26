---
title: embeddedSIMActivationCodePoolAssignment の更新
description: embeddedSIMActivationCodePoolAssignment オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4fa2030d6b2b8fb260c28d94caff031ec2db0ae1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164450"
---
# <a name="update-embeddedsimactivationcodepoolassignment"></a><span data-ttu-id="b23b5-103">embeddedSIMActivationCodePoolAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="b23b5-103">Update embeddedSIMActivationCodePoolAssignment</span></span>

> <span data-ttu-id="b23b5-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b23b5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b23b5-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b23b5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b23b5-106">[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b23b5-106">Update the properties of a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b23b5-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="b23b5-107">Prerequisites</span></span>
<span data-ttu-id="b23b5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b23b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b23b5-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b23b5-110">Permission type</span></span>|<span data-ttu-id="b23b5-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b23b5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b23b5-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b23b5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b23b5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b23b5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b23b5-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b23b5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b23b5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b23b5-115">Not supported.</span></span>|
|<span data-ttu-id="b23b5-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b23b5-116">Application</span></span>|<span data-ttu-id="b23b5-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b23b5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b23b5-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b23b5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="b23b5-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b23b5-119">Request headers</span></span>
|<span data-ttu-id="b23b5-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b23b5-120">Header</span></span>|<span data-ttu-id="b23b5-121">値</span><span class="sxs-lookup"><span data-stu-id="b23b5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b23b5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b23b5-122">Authorization</span></span>|<span data-ttu-id="b23b5-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b23b5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b23b5-124">承諾</span><span class="sxs-lookup"><span data-stu-id="b23b5-124">Accept</span></span>|<span data-ttu-id="b23b5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b23b5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b23b5-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="b23b5-126">Request body</span></span>
<span data-ttu-id="b23b5-127">要求本文で、 [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b23b5-127">In the request body, supply a JSON representation for the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

<span data-ttu-id="b23b5-128">次の表に、 [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b23b5-128">The following table shows the properties that are required when you create the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).</span></span>

|<span data-ttu-id="b23b5-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b23b5-129">Property</span></span>|<span data-ttu-id="b23b5-130">型</span><span class="sxs-lookup"><span data-stu-id="b23b5-130">Type</span></span>|<span data-ttu-id="b23b5-131">説明</span><span class="sxs-lookup"><span data-stu-id="b23b5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b23b5-132">id</span><span class="sxs-lookup"><span data-stu-id="b23b5-132">id</span></span>|<span data-ttu-id="b23b5-133">String</span><span class="sxs-lookup"><span data-stu-id="b23b5-133">String</span></span>|<span data-ttu-id="b23b5-134">埋め込まれている SIM ライセンス認証コードプールの割り当ての一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="b23b5-134">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="b23b5-135">作成時に割り当てられたシステム生成値。</span><span class="sxs-lookup"><span data-stu-id="b23b5-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="b23b5-136">target</span><span class="sxs-lookup"><span data-stu-id="b23b5-136">target</span></span>|[<span data-ttu-id="b23b5-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b23b5-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b23b5-138">埋め込まれた SIM アクティブ化コードプールの対象となるグループの種類。</span><span class="sxs-lookup"><span data-stu-id="b23b5-138">The type of groups targeted by the embedded SIM activation code pool.</span></span>|



## <a name="response"></a><span data-ttu-id="b23b5-139">応答</span><span class="sxs-lookup"><span data-stu-id="b23b5-139">Response</span></span>
<span data-ttu-id="b23b5-140">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b23b5-140">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b23b5-141">例</span><span class="sxs-lookup"><span data-stu-id="b23b5-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="b23b5-142">要求</span><span class="sxs-lookup"><span data-stu-id="b23b5-142">Request</span></span>
<span data-ttu-id="b23b5-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b23b5-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="b23b5-144">応答</span><span class="sxs-lookup"><span data-stu-id="b23b5-144">Response</span></span>
<span data-ttu-id="b23b5-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b23b5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




