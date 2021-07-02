Project for Cognitive Computing and Artificial Intelligence of Germano Giuseppe, Di Blasi Kristian, Impalà Antonio. 

Commands to play the tests:

	Domain-IL:

		Rot-mnist with DER:
			python3 utils/main.py --model der --load_best_args --dataset rot-mnist --buffer_size 200
			python3 utils/main.py --model der --load_best_args --dataset rot-mnist --buffer_size 500
			python3 utils/main.py --model der --load_best_args --dataset rot-mnist --buffer_size 5120

		Rot-mnist with DERPP:
			python3 utils/main.py --model derpp --load_best_args --dataset rot-mnist --buffer_size 200
			python3 utils/main.py --model derpp --load_best_args --dataset rot-mnist --buffer_size 500
			python3 utils/main.py --model derpp --load_best_args --dataset rot-mnist --buffer_size 5120

		Perm-mnist with DER:
			python3 utils/main.py --model der --load_best_args --dataset perm-mnist --buffer_size 200
			python3 utils/main.py --model der --load_best_args --dataset perm-mnist --buffer_size 500
			python3 utils/main.py --model der --load_best_args --dataset perm-mnist --buffer_size 5120
	
		Perm-mnist with DERPP:
			python3 utils/main.py --model derpp --load_best_args --dataset perm-mnist --buffer_size 200
			python3 utils/main.py --model derpp --load_best_args --dataset perm-mnist --buffer_size 500
			python3 utils/main.py --model derpp --load_best_args --dataset perm-mnist --buffer_size 5120

	Class-IL and Task-IL:

		Seq-mnist with DER:
			python3 utils/main.py --model der --load_best_args --dataset seq-mnist --buffer_size 200
			python3 utils/main.py --model der --load_best_args --dataset seq-mnist --buffer_size 500
			python3 utils/main.py --model der --load_best_args --dataset seq-mnist --buffer_size 5120
		
		Seq-mnist with DERPP:
			python3 utils/main.py --model derpp --load_best_args --dataset seq-mnist --buffer_size 200
			python3 utils/main.py --model derpp --load_best_args --dataset seq-mnist --buffer_size 500
			python3 utils/main.py --model derpp --load_best_args --dataset seq-mnist --buffer_size 5120

	Generic Continual Learning:

		Mnist-360 with DER:
			python3 utils/main.py --model der --load_best_args --dataset mnist-360 --buffer_size 200
			python3 utils/main.py --model der --load_best_args --dataset mnist-360 --buffer_size 500
			python3 utils/main.py --model der --load_best_args --dataset mnist-360 --buffer_size 1000

		Mnist-360 with DERPP:
			python3 utils/main.py --model derpp --load_best_args --dataset mnist-360 --buffer_size 200
			python3 utils/main.py --model derpp --load_best_args --dataset mnist-360 --buffer_size 500
			python3 utils/main.py --model derpp --load_best_args --dataset mnist-360 --buffer_size 1000

	Other tests:
	
		Seq-mnist with DER (without best args):
			python3 utils/main.py --model der --dataset seq-mnist --buffer_size 500 --lr 0.001 --batch_size 8 --n_epochs 10 --minibatch_size 8 --alpha 1.0
			python3 utils/main.py --model der --dataset seq-mnist --buffer_size 500 --lr 0.001 --batch_size 10 --n_epochs 1 --minibatch_size 128 --alpha 1.0
