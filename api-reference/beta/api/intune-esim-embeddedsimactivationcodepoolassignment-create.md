---
title: embeddedSIMActivationCodePoolAssignment を作成する
description: 新しい embeddedSIMActivationCodePoolAssignment オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 67e124fafcd46519667373dc45b1fe38084d3128
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30971914"
---
# <a name="create-embeddedsimactivationcodepoolassignment"></a><span data-ttu-id="37f15-103">embeddedSIMActivationCodePoolAssignment を作成する</span><span class="sxs-lookup"><span data-stu-id="37f15-103">Create embeddedSIMActivationCodePoolAssignment</span></span>

> <span data-ttu-id="37f15-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="37f15-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37f15-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="37f15-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37f15-106">新しい[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="37f15-106">Create a new [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37f15-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="37f15-107">Prerequisites</span></span>
<span data-ttu-id="37f15-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="37f15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37f15-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="37f15-110">Permission type</span></span>|<span data-ttu-id="37f15-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="37f15-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37f15-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="37f15-112">Delegated (work or school account)</span></span>|<span data-ttu-id="37f15-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37f15-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="37f15-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="37f15-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37f15-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="37f15-115">Not supported.</span></span>|
|<span data-ttu-id="37f15-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="37f15-116">Application</span></span>|<span data-ttu-id="37f15-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="37f15-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37f15-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="37f15-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="37f15-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="37f15-119">Request headers</span></span>
|<span data-ttu-id="37f15-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="37f15-120">Header</span></span>|<span data-ttu-id="37f15-121">値</span><span class="sxs-lookup"><span data-stu-id="37f15-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37f15-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="37f15-122">Authorization</span></span>|<span data-ttu-id="37f15-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="37f15-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37f15-124">承諾</span><span class="sxs-lookup"><span data-stu-id="37f15-124">Accept</span></span>|<span data-ttu-id="37f15-125">application/json</span><span class="sxs-lookup"><span data-stu-id="37f15-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37f15-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="37f15-126">Request body</span></span>
<span data-ttu-id="37f15-127">要求本文で、embeddedSIMActivationCodePoolAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="37f15-127">In the request body, supply a JSON representation for the embeddedSIMActivationCodePoolAssignment object.</span></span>

<span data-ttu-id="37f15-128">次の表に、embeddedSIMActivationCodePoolAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="37f15-128">The following table shows the properties that are required when you create the embeddedSIMActivationCodePoolAssignment.</span></span>

|<span data-ttu-id="37f15-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="37f15-129">Property</span></span>|<span data-ttu-id="37f15-130">型</span><span class="sxs-lookup"><span data-stu-id="37f15-130">Type</span></span>|<span data-ttu-id="37f15-131">説明</span><span class="sxs-lookup"><span data-stu-id="37f15-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37f15-132">id</span><span class="sxs-lookup"><span data-stu-id="37f15-132">id</span></span>|<span data-ttu-id="37f15-133">String</span><span class="sxs-lookup"><span data-stu-id="37f15-133">String</span></span>|<span data-ttu-id="37f15-134">埋め込まれている SIM ライセンス認証コードプールの割り当ての一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="37f15-134">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="37f15-135">作成時に割り当てられたシステム生成値。</span><span class="sxs-lookup"><span data-stu-id="37f15-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="37f15-136">target</span><span class="sxs-lookup"><span data-stu-id="37f15-136">target</span></span>|[<span data-ttu-id="37f15-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="37f15-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="37f15-138">埋め込まれた SIM アクティブ化コードプールの対象となるグループの種類。</span><span class="sxs-lookup"><span data-stu-id="37f15-138">The type of groups targeted by the embedded SIM activation code pool.</span></span>|



## <a name="response"></a><span data-ttu-id="37f15-139">応答</span><span class="sxs-lookup"><span data-stu-id="37f15-139">Response</span></span>
<span data-ttu-id="37f15-140">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="37f15-140">If successful, this method returns a `201 Created` response code and a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37f15-141">例</span><span class="sxs-lookup"><span data-stu-id="37f15-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="37f15-142">要求</span><span class="sxs-lookup"><span data-stu-id="37f15-142">Request</span></span>
<span data-ttu-id="37f15-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="37f15-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="37f15-144">応答</span><span class="sxs-lookup"><span data-stu-id="37f15-144">Response</span></span>
<span data-ttu-id="37f15-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="37f15-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




