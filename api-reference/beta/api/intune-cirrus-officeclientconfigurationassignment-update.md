---
title: OfficeClientConfigurationAssignment の更新
description: OfficeClientConfigurationAssignment オブジェクトのプロパティを更新します。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: af97473ae7c72d3d107d2346e08caa7f264bc285
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420799"
---
# <a name="update-officeclientconfigurationassignment"></a><span data-ttu-id="e3038-103">OfficeClientConfigurationAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="e3038-103">Update officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="e3038-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3038-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3038-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e3038-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3038-106">[OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e3038-106">Update the properties of a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3038-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e3038-107">Prerequisites</span></span>
<span data-ttu-id="e3038-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3038-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3038-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e3038-110">Permission type</span></span>|<span data-ttu-id="e3038-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e3038-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3038-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e3038-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e3038-113">**TODO: スコープを決定する**</span><span class="sxs-lookup"><span data-stu-id="e3038-113">**TODO: Determine scopes**</span></span>|
|<span data-ttu-id="e3038-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e3038-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3038-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3038-115">Not supported.</span></span>|
|<span data-ttu-id="e3038-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e3038-116">Application</span></span>|<span data-ttu-id="e3038-117">\* \* TODO: 範囲を決定します \* \*</span><span class="sxs-lookup"><span data-stu-id="e3038-117">\*\*TODO: Determine scopes \*\*</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3038-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e3038-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="e3038-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3038-119">Request headers</span></span>
|<span data-ttu-id="e3038-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3038-120">Header</span></span>|<span data-ttu-id="e3038-121">値</span><span class="sxs-lookup"><span data-stu-id="e3038-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3038-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3038-122">Authorization</span></span>|<span data-ttu-id="e3038-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e3038-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3038-124">承諾</span><span class="sxs-lookup"><span data-stu-id="e3038-124">Accept</span></span>|<span data-ttu-id="e3038-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e3038-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3038-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e3038-126">Request body</span></span>
<span data-ttu-id="e3038-127">要求本文で、 [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e3038-127">In the request body, supply a JSON representation for the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

<span data-ttu-id="e3038-128">次の表に、 [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e3038-128">The following table shows the properties that are required when you create the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span></span>

|<span data-ttu-id="e3038-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e3038-129">Property</span></span>|<span data-ttu-id="e3038-130">型</span><span class="sxs-lookup"><span data-stu-id="e3038-130">Type</span></span>|<span data-ttu-id="e3038-131">説明</span><span class="sxs-lookup"><span data-stu-id="e3038-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3038-132">id</span><span class="sxs-lookup"><span data-stu-id="e3038-132">id</span></span>|<span data-ttu-id="e3038-133">String</span><span class="sxs-lookup"><span data-stu-id="e3038-133">String</span></span>|<span data-ttu-id="e3038-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e3038-134">Not yet documented</span></span>|
|<span data-ttu-id="e3038-135">target</span><span class="sxs-lookup"><span data-stu-id="e3038-135">target</span></span>|[<span data-ttu-id="e3038-136">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e3038-136">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="e3038-137">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e3038-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e3038-138">応答</span><span class="sxs-lookup"><span data-stu-id="e3038-138">Response</span></span>
<span data-ttu-id="e3038-139">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e3038-139">If successful, this method returns a `200 OK` response code and an updated [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3038-140">例</span><span class="sxs-lookup"><span data-stu-id="e3038-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3038-141">要求</span><span class="sxs-lookup"><span data-stu-id="e3038-141">Request</span></span>
<span data-ttu-id="e3038-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e3038-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
Content-type: application/json
Content-length: 98

{
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="e3038-143">応答</span><span class="sxs-lookup"><span data-stu-id="e3038-143">Response</span></span>
<span data-ttu-id="e3038-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e3038-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
  "id": "804730f3-30f3-8047-f330-4780f3304780",
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```






