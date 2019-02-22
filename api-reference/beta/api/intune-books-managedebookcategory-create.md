---
title: managedebookcategory の作成
description: 新しい managedebookcategory オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fd23f14bab5db4ef0d0fbae7f3ff2d752a28595c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147636"
---
# <a name="create-managedebookcategory"></a><span data-ttu-id="f6d1b-103">managedebookcategory の作成</span><span class="sxs-lookup"><span data-stu-id="f6d1b-103">Create managedEBookCategory</span></span>

> <span data-ttu-id="f6d1b-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f6d1b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6d1b-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f6d1b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6d1b-106">新しい[managedebookcategory](../resources/intune-books-managedebookcategory.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f6d1b-106">Create a new [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6d1b-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f6d1b-107">Prerequisites</span></span>
<span data-ttu-id="f6d1b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f6d1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f6d1b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f6d1b-110">Permission type</span></span>|<span data-ttu-id="f6d1b-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f6d1b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6d1b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f6d1b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f6d1b-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6d1b-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f6d1b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f6d1b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6d1b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f6d1b-115">Not supported.</span></span>|
|<span data-ttu-id="f6d1b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f6d1b-116">Application</span></span>|<span data-ttu-id="f6d1b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f6d1b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6d1b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f6d1b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBookCategories
POST /deviceAppManagement/managedEBooks/{managedEBookId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="f6d1b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f6d1b-119">Request headers</span></span>
|<span data-ttu-id="f6d1b-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f6d1b-120">Header</span></span>|<span data-ttu-id="f6d1b-121">値</span><span class="sxs-lookup"><span data-stu-id="f6d1b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6d1b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6d1b-122">Authorization</span></span>|<span data-ttu-id="f6d1b-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f6d1b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6d1b-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f6d1b-124">Accept</span></span>|<span data-ttu-id="f6d1b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f6d1b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6d1b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f6d1b-126">Request body</span></span>
<span data-ttu-id="f6d1b-127">要求本文で、managedebookcategory オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f6d1b-127">In the request body, supply a JSON representation for the managedEBookCategory object.</span></span>

<span data-ttu-id="f6d1b-128">次の表に、managedebookcategory の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f6d1b-128">The following table shows the properties that are required when you create the managedEBookCategory.</span></span>

|<span data-ttu-id="f6d1b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f6d1b-129">Property</span></span>|<span data-ttu-id="f6d1b-130">型</span><span class="sxs-lookup"><span data-stu-id="f6d1b-130">Type</span></span>|<span data-ttu-id="f6d1b-131">説明</span><span class="sxs-lookup"><span data-stu-id="f6d1b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6d1b-132">id</span><span class="sxs-lookup"><span data-stu-id="f6d1b-132">id</span></span>|<span data-ttu-id="f6d1b-133">String</span><span class="sxs-lookup"><span data-stu-id="f6d1b-133">String</span></span>|<span data-ttu-id="f6d1b-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f6d1b-134">The key of the entity.</span></span>|
|<span data-ttu-id="f6d1b-135">displayName</span><span class="sxs-lookup"><span data-stu-id="f6d1b-135">displayName</span></span>|<span data-ttu-id="f6d1b-136">String</span><span class="sxs-lookup"><span data-stu-id="f6d1b-136">String</span></span>|<span data-ttu-id="f6d1b-137">eBook カテゴリの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="f6d1b-137">The name of the eBook category.</span></span>|
|<span data-ttu-id="f6d1b-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f6d1b-138">lastModifiedDateTime</span></span>|<span data-ttu-id="f6d1b-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6d1b-139">DateTimeOffset</span></span>|<span data-ttu-id="f6d1b-140">managedebookcategory が最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="f6d1b-140">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="f6d1b-141">応答</span><span class="sxs-lookup"><span data-stu-id="f6d1b-141">Response</span></span>
<span data-ttu-id="f6d1b-142">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[managedebookcategory](../resources/intune-books-managedebookcategory.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f6d1b-142">If successful, this method returns a `201 Created` response code and a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6d1b-143">例</span><span class="sxs-lookup"><span data-stu-id="f6d1b-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6d1b-144">要求</span><span class="sxs-lookup"><span data-stu-id="f6d1b-144">Request</span></span>
<span data-ttu-id="f6d1b-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f6d1b-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="f6d1b-146">応答</span><span class="sxs-lookup"><span data-stu-id="f6d1b-146">Response</span></span>
<span data-ttu-id="f6d1b-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f6d1b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 215

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "id": "3c71fb14-fb14-3c71-14fb-713c14fb713c",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




