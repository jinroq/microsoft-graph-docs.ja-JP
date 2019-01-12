---
title: Planner でオーダー ヒントを使用する
description: '`)'
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: fa518e3820437ec02ee2b28e1b9a93fab3d4b100
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977690"
---
# <a name="using-order-hints-in-planner"></a><span data-ttu-id="f0eae-103">Planner でオーダー ヒントを使用する</span><span class="sxs-lookup"><span data-stu-id="f0eae-103">Using order hints in Planner</span></span>

> <span data-ttu-id="f0eae-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f0eae-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f0eae-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0eae-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f0eae-p102">オーダー ヒントによって、Planner 内のオブジェクトの並べ替え順序を特定します。オーダー ヒントの値は文字列です。クライアントは項目の順序を特定するため、文字の序数値に基づいて文字列を並べ替えることができます。文字の序数値に違いが発生するまで、または文字列の終わりまで、文字列の先頭から文字を比較します。後者の場合、短い方の文字列を長い文字列より前に並べ替えます。値には、32 (スペース) から 126 (`~`) の序数のうち、どの文字でも含めることができます</span><span class="sxs-lookup"><span data-stu-id="f0eae-p102">Objects in Planner identify their sort order by order hints. The order hint values are strings. The clients can sort the strings based on ordinal value of characters in them to identify the order of items. The characters are compared from the beginning of the string, until a difference is encountered in the ordinal values of characters, or one string ends, in which case the shorter string would be sorted before the longer. The values can contain any character between ordinals 32 (space) and 126 (`~`)</span></span>

<span data-ttu-id="f0eae-p103">一例として、オーダー ヒント `a` (序数値 97) を持つ項目は、オーダー ヒント `z` (序数値 122) を持つ別の項目より前に配置されます。オーダー ヒント `abc` (序数値 97、98、99) を持つ項目は、オーダー ヒント `abd` (序数値 97、98、100) を持つ別の項目より前に配置されます。オーダー ヒント `a` を持つ項目は、オーダー ヒント `ab` を持つ別の項目より前に配置されますが、これは存在するすべての文字が同じであり、`a` の方が短いためです。</span><span class="sxs-lookup"><span data-stu-id="f0eae-p103">As an example, an item with order hint `a` (ordinal value 97) would be placed before another item with order hint `z` (ordinal value 122). An item with order hint `abc` (ordinal values 97, 98, 99), would be placed before another item with order hint `abd` (ordinal values 97, 98, 100). An item with order hint `a` would be placed before another item with order hint `ab` since all existing characters are the same, and `a` is shorter.</span></span>

<span data-ttu-id="f0eae-p104">このサービスにより、すべてのオーダー ヒントの値を計算します。クライアントは、2 つの項目間を移動した項目のオーダー ヒントを指定することによって、項目を並べ替えることができます。オーダー ヒントを次の値に設定します。`<previous order hint> <next order hint>!`、ここでは新しく要求した場所の前に来る項目のオーダー ヒントによって `<previous order hint>` が置き換えられ、新しく要求した場所の後に来る項目のオーダー ヒントによって `<next order hint>` が置き換えられます。これらのオーダー ヒントの値の間には空白文字があり、値全体の後に `!` が付きます。いずれの項目も存在しない場合は、代わりに空の文字列を使用する必要があります。この値は以前の計算で構成することもでき、オーダー ヒントを返したサービスと全く同じように項目を並べ替えるためにクライアントで使用することもできます。更新プログラムでクライアントがこれらの値を送信したら、このサービスは要求された場所で並べ替えを行う短い値を計算します。</span><span class="sxs-lookup"><span data-stu-id="f0eae-p104">The values for all order hints are calculated by the service. The client can reorder items by specifying the order hint for the item that got moved between two items with by setting the order hint to the following value: `<previous order hint> <next order hint>!`, where `<previous order hint>` is to be replaced by the order hint of the item that comes before the new desired location, and `<next order hint>` is to be replaced by the order hint of the item that comes after the new desired location. There is a space character between these order hint values, and the entire value is suffixed with `!`. If either item isn't present, empty string should be used instead. This value can also be composed of previous calculations, and can be used in the client to sort items exactly like service returned order hints. Once the client sends these values in an update, the service will calculate a short value that sorts in the desired location.</span></span>

> <span data-ttu-id="f0eae-120">**注:** 次の例では、実際の順序のヒントの値が単一引用符で囲まれた (`'`) をわかりやすく、ただしこれらのデータの一部ではないしサービスに送信する必要がありません。</span><span class="sxs-lookup"><span data-stu-id="f0eae-120">**Note:** In the following examples, the actual order hint values are surrounded in single quote characters (`'`) for clarity, however these are not part of the data, and must not be sent to the service.</span></span>
 
<span data-ttu-id="f0eae-121">たとえば、以下のオーダー ヒントの並べ替えのリストについて検討します。</span><span class="sxs-lookup"><span data-stu-id="f0eae-121">As an example, consider the following list of sorted order hints:</span></span>

1. <span data-ttu-id="f0eae-122">項目 1 (オーダー ヒント: `'5637'`)</span><span class="sxs-lookup"><span data-stu-id="f0eae-122">Item 1 (Order Hint: `'5637'`)</span></span>
2. <span data-ttu-id="f0eae-123">項目 2 (オーダー ヒント: `'adhg'`)</span><span class="sxs-lookup"><span data-stu-id="f0eae-123">Item 2 (Order Hint: `'adhg'`)</span></span>

<span data-ttu-id="f0eae-124">項目 3 を項目 1 の前に配置し、次に項目 4 を項目 1 と項目 2 の間に配置します。次いで項目 5 を項目 2 の後に配置すれば、クライアント上で以下のオーダー ヒントが作成されます。</span><span class="sxs-lookup"><span data-stu-id="f0eae-124">Placing an Item 3 before Item 1, then placing item 4 between Item 1 and Item 2, and then placing item 5 after Item 2, would create the following order hints on the client.</span></span> 

1. <span data-ttu-id="f0eae-125">項目 3 (オーダー ヒント: `' 5637!'`)</span><span class="sxs-lookup"><span data-stu-id="f0eae-125">Item 3 (Order Hint: `' 5637!'`)</span></span>
2. <span data-ttu-id="f0eae-126">項目 1 (オーダー ヒント: `'5637'`)</span><span class="sxs-lookup"><span data-stu-id="f0eae-126">Item 1 (Order Hint: `'5637'`)</span></span>
3. <span data-ttu-id="f0eae-127">項目 4 (オーダー ヒント: `'5637 adhg!'`)</span><span class="sxs-lookup"><span data-stu-id="f0eae-127">Item 4 (Order Hint: `'5637 adhg!'`)</span></span>
4. <span data-ttu-id="f0eae-128">項目 2 (オーダー ヒント: `'adhg'`)</span><span class="sxs-lookup"><span data-stu-id="f0eae-128">Item 2 (Order Hint: `'adhg'`)</span></span>
5. <span data-ttu-id="f0eae-129">項目 5 (オーダー ヒント: `'adhg !'`)</span><span class="sxs-lookup"><span data-stu-id="f0eae-129">Item 5 (Order Hint: `'adhg !'`)</span></span>

<span data-ttu-id="f0eae-130">次に、項目 1 をリストの末尾に移動すると、次のオーダー ヒントが生成されます。</span><span class="sxs-lookup"><span data-stu-id="f0eae-130">Then, moving item 1 to the end of the list would generate:</span></span>

1. <span data-ttu-id="f0eae-131">項目 3 (オーダー ヒント: `' 5637!'`)</span><span class="sxs-lookup"><span data-stu-id="f0eae-131">Item 3 (Order Hint: `' 5637!'`)</span></span>
2. <span data-ttu-id="f0eae-132">項目 4 (オーダー ヒント: `'5637 adhg!'`)</span><span class="sxs-lookup"><span data-stu-id="f0eae-132">Item 4 (Order Hint: `'5637 adhg!'`)</span></span>
3. <span data-ttu-id="f0eae-133">項目 2 (オーダー ヒント: `'adhg'`)</span><span class="sxs-lookup"><span data-stu-id="f0eae-133">Item 2 (Order Hint: `'adhg'`)</span></span>
4. <span data-ttu-id="f0eae-134">項目 5 (オーダー ヒント: `'adhg !'`)</span><span class="sxs-lookup"><span data-stu-id="f0eae-134">Item 5 (Order Hint: `'adhg !'`)</span></span>
5. <span data-ttu-id="f0eae-135">項目 1 (オーダー ヒント: `'adhg ! !'`)</span><span class="sxs-lookup"><span data-stu-id="f0eae-135">Item 1 (Order Hint: `'adhg ! !'`)</span></span>

<span data-ttu-id="f0eae-136">最後に、項目 5 を項目 3 と項目 4 の間に移動すると、次のオーダー ヒントが生成されます。</span><span class="sxs-lookup"><span data-stu-id="f0eae-136">Finally moving Item 5 between Item 3 and Item 4 would generate:</span></span>

1. <span data-ttu-id="f0eae-137">項目 3 (オーダー ヒント: `' 5637!'`)</span><span class="sxs-lookup"><span data-stu-id="f0eae-137">Item 3 (Order Hint: `' 5637!'`)</span></span>
2. <span data-ttu-id="f0eae-138">項目 5 (オーダー ヒント: `' 5637! 5637 adhg!!'`)</span><span class="sxs-lookup"><span data-stu-id="f0eae-138">Item 5 (Order Hint: `' 5637! 5637 adhg!!'`)</span></span>
3. <span data-ttu-id="f0eae-139">項目 4 (オーダー ヒント: `'5637 adhg!'`)</span><span class="sxs-lookup"><span data-stu-id="f0eae-139">Item 4 (Order Hint: `'5637 adhg!'`)</span></span>
4. <span data-ttu-id="f0eae-140">項目 2 (オーダー ヒント: `'adhg'`)</span><span class="sxs-lookup"><span data-stu-id="f0eae-140">Item 2 (Order Hint: `'adhg'`)</span></span>
5. <span data-ttu-id="f0eae-141">項目 1 (オーダー ヒント: `'adhg ! !'`)</span><span class="sxs-lookup"><span data-stu-id="f0eae-141">Item 1 (Order Hint: `'adhg ! !'`)</span></span>

<span data-ttu-id="f0eae-142">ヒントの値を順にこれらの変更が修正プログラムの要求のサービスに送信されると、サービスはクライアントが意図した順番を保持する適切な値を計算します。</span><span class="sxs-lookup"><span data-stu-id="f0eae-142">When these changes to order hint values are sent to the service in patch requests, the service will calculate proper values that keep the order intended by the client.</span></span> <span data-ttu-id="f0eae-143">クライアントは、イミディ エイト場合に、値を取得できる、`Prefer: return=representation`の優先順位ヘッダーが指定されている、`PATCH`の要求。</span><span class="sxs-lookup"><span data-stu-id="f0eae-143">The client can obtain the values immediate if the `Prefer: return=representation` preference header is specified in the `PATCH` requests.</span></span> <span data-ttu-id="f0eae-144">上記の場合の値は、次のように表示されます (実際の値は異なる場合があります)。</span><span class="sxs-lookup"><span data-stu-id="f0eae-144">The values for the case above may look like the following (the actual values may differ).</span></span> 

1. <span data-ttu-id="f0eae-145">項目 3 (オーダー ヒント: `'432b'`)</span><span class="sxs-lookup"><span data-stu-id="f0eae-145">Item 3 (Order Hint: `'432b'`)</span></span>
2. <span data-ttu-id="f0eae-146">項目 5 (オーダー ヒント: `'6F"#'`)</span><span class="sxs-lookup"><span data-stu-id="f0eae-146">Item 5 (Order Hint: `'6F"#'`)</span></span>
3. <span data-ttu-id="f0eae-147">項目 4 (オーダー ヒント: `'7A$6'`)</span><span class="sxs-lookup"><span data-stu-id="f0eae-147">Item 4 (Order Hint: `'7A$6'`)</span></span>
4. <span data-ttu-id="f0eae-148">項目 2 (オーダー ヒント: `'adhg'`)</span><span class="sxs-lookup"><span data-stu-id="f0eae-148">Item 2 (Order Hint: `'adhg'`)</span></span>
5. <span data-ttu-id="f0eae-149">項目 1 (オーダー ヒント: `'de5%'`)</span><span class="sxs-lookup"><span data-stu-id="f0eae-149">Item 1 (Order Hint: `'de5%'`)</span></span>

<span data-ttu-id="f0eae-p106">リストの最初の項目を作成する場合、前または次の項目がいずれも存在しないため、オーダー ヒントを ` !` として指定することができます。ただし、項目の作成時にオーダー ヒントの値が指定されない場合、そうする必要はありません。これは、サービスが項目のすべてのオーダー ヒントの値を自動生成するためです。次の例は、以前に空白だったリストに項目を配置する場合、オーダー ヒントを使用する必要があることを示しています。最初の項目を追加します。</span><span class="sxs-lookup"><span data-stu-id="f0eae-p106">Order Hints can be specified for creating the first item in the list as ` !`, since neither a previous or a next item exists in that case, however this is unnecessary, as the service will auto-generate values for all order hint values on items if they are not specified during creation of the item. Following example illustrates the order hints should be used when placing items in a previously empty list. Add the first item:</span></span>

1. <span data-ttu-id="f0eae-153">項目 1 (オーダー ヒント: `' !'`)</span><span class="sxs-lookup"><span data-stu-id="f0eae-153">Item 1 (Order Hint: `' !'`)</span></span>

<span data-ttu-id="f0eae-154">2 番目の項目を先頭に追加します。</span><span class="sxs-lookup"><span data-stu-id="f0eae-154">Add the second item to top:</span></span>

1. <span data-ttu-id="f0eae-155">項目 2 (オーダー ヒント: `'  !!'`)</span><span class="sxs-lookup"><span data-stu-id="f0eae-155">Item 2 (Order Hint: `'  !!'`)</span></span>
2. <span data-ttu-id="f0eae-156">項目 1 (オーダー ヒント: `' !'`)</span><span class="sxs-lookup"><span data-stu-id="f0eae-156">Item 1 (Order Hint: `' !'`)</span></span>

<span data-ttu-id="f0eae-157">3 番目の項目を一番下に追加します。</span><span class="sxs-lookup"><span data-stu-id="f0eae-157">Add the third item to bottom:</span></span>

1. <span data-ttu-id="f0eae-158">項目 2 (オーダー ヒント: `'  !!'`)</span><span class="sxs-lookup"><span data-stu-id="f0eae-158">Item 2 (Order Hint: `'  !!'`)</span></span>
2. <span data-ttu-id="f0eae-159">項目 1 (オーダー ヒント: `' !'`)</span><span class="sxs-lookup"><span data-stu-id="f0eae-159">Item 1 (Order Hint: `' !'`)</span></span>
3. <span data-ttu-id="f0eae-160">項目 3 (オーダー ヒント: `' ! !'`)</span><span class="sxs-lookup"><span data-stu-id="f0eae-160">Item 3 (Order Hint: `' ! !'`)</span></span>







