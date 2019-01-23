---
title: ManagedEBookCategory を更新します。
description: ManagedEBookCategory オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 832fb3f2ddc180a88a21d9484057332800e062a5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398332"
---
# <a name="update-managedebookcategory"></a><span data-ttu-id="ee457-103">ManagedEBookCategory を更新します。</span><span class="sxs-lookup"><span data-stu-id="ee457-103">Update managedEBookCategory</span></span>

> <span data-ttu-id="ee457-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ee457-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ee457-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee457-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ee457-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ee457-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee457-107">[ManagedEBookCategory](../resources/intune-books-managedebookcategory.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ee457-107">Update the properties of a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee457-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="ee457-108">Prerequisites</span></span>
<span data-ttu-id="ee457-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ee457-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ee457-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ee457-111">Permission type</span></span>|<span data-ttu-id="ee457-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ee457-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee457-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ee457-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ee457-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee457-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ee457-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ee457-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee457-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee457-116">Not supported.</span></span>|
|<span data-ttu-id="ee457-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ee457-117">Application</span></span>|<span data-ttu-id="ee457-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee457-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee457-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ee457-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/categories/{managedEBookCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="ee457-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ee457-120">Request headers</span></span>
|<span data-ttu-id="ee457-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ee457-121">Header</span></span>|<span data-ttu-id="ee457-122">値</span><span class="sxs-lookup"><span data-stu-id="ee457-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee457-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee457-123">Authorization</span></span>|<span data-ttu-id="ee457-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ee457-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee457-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ee457-125">Accept</span></span>|<span data-ttu-id="ee457-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ee457-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee457-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ee457-127">Request body</span></span>
<span data-ttu-id="ee457-128">要求の本文に[managedEBookCategory](../resources/intune-books-managedebookcategory.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="ee457-128">In the request body, supply a JSON representation for the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

<span data-ttu-id="ee457-129">[ManagedEBookCategory](../resources/intune-books-managedebookcategory.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="ee457-129">The following table shows the properties that are required when you create the [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span></span>

|<span data-ttu-id="ee457-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ee457-130">Property</span></span>|<span data-ttu-id="ee457-131">型</span><span class="sxs-lookup"><span data-stu-id="ee457-131">Type</span></span>|<span data-ttu-id="ee457-132">説明</span><span class="sxs-lookup"><span data-stu-id="ee457-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee457-133">id</span><span class="sxs-lookup"><span data-stu-id="ee457-133">id</span></span>|<span data-ttu-id="ee457-134">String</span><span class="sxs-lookup"><span data-stu-id="ee457-134">String</span></span>|<span data-ttu-id="ee457-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ee457-135">The key of the entity.</span></span>|
|<span data-ttu-id="ee457-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ee457-136">displayName</span></span>|<span data-ttu-id="ee457-137">String</span><span class="sxs-lookup"><span data-stu-id="ee457-137">String</span></span>|<span data-ttu-id="ee457-138">EBook カテゴリの名前です。</span><span class="sxs-lookup"><span data-stu-id="ee457-138">The name of the eBook category.</span></span>|
|<span data-ttu-id="ee457-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee457-139">lastModifiedDateTime</span></span>|<span data-ttu-id="ee457-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee457-140">DateTimeOffset</span></span>|<span data-ttu-id="ee457-141">日付と時刻、ManagedEBookCategory が最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="ee457-141">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="ee457-142">応答</span><span class="sxs-lookup"><span data-stu-id="ee457-142">Response</span></span>
<span data-ttu-id="ee457-143">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[managedEBookCategory](../resources/intune-books-managedebookcategory.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="ee457-143">If successful, this method returns a `200 OK` response code and an updated [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee457-144">例</span><span class="sxs-lookup"><span data-stu-id="ee457-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee457-145">要求</span><span class="sxs-lookup"><span data-stu-id="ee457-145">Request</span></span>
<span data-ttu-id="ee457-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ee457-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="ee457-147">応答</span><span class="sxs-lookup"><span data-stu-id="ee457-147">Response</span></span>
<span data-ttu-id="ee457-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ee457-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 215

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "id": "3c71fb14-fb14-3c71-14fb-713c14fb713c",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




